---
layout: post
title: Python and Paraview for batch processing
date: 2025-01-08 20:57:00
description:
tags: python paraview batch
categories: python paraview
featured: true
---

I just tested a super useful feature of [Paraview](https://github.com/Kitware/ParaView). In a nutshell, I have been using paraview in the context of the research project Woodseer, for 3d rendering Xrays and their annotations.

Unfortunately, I had to generate illustrations from a batch of data and doing so
from the GUI is not easy.

Fortunaly, Paraview allows to record all the operations performed on the GUI and
export all of these operations as a python script. The script is hardcoding the
data filenames to be processed but it is only about changing few lines at the
beginning of the script and you have a script able to batch process a collection
of data.

To record your interactions with Paraview, just clicking `Tools / Start trace`.
Then you proceed with paraviex, adding your data, manipulating the 3d display,
view point, colors, etc... Once done, just click on `Tools/Stop trace` and
paraview will give you the equivalent python script for doing exactly the same
operations. As a bonus, at the end of the script, we are provided sample codes
for either displaying the output or even producing a screenshot.

To run the script from your console, we need to use the `pvpython` interpreter
which I believe contains its virtual environment for accessing the paraview
python library.

```bash
pvpython paraplot_bil.py /opt/Datasets/Woodseer/Slicing/Sapin/4396
```

And there you are :

{% include figure.liquid path="assets/img/bil_4396.png" title="Example rendering using paraview python scripting" class="img-fluid rounded z-depth-1" zoomable=true %}

The python script that has been produced by the paraview export is given below :

```python
# trace generated using paraview version 5.13.0
# import paraview
# paraview.compatibility.major = 5
# paraview.compatibility.minor = 13

#### import the simple module from the paraview
import sys
import pathlib
from paraview.simple import *

#### disable automatic camera reset on 'Show'
paraview.simple._DisableFirstRenderCameraReset()

if len(sys.argv) != 2:
    print("Usage: python paraplot_compare.py <xraydirw>")
    sys.exit(1)
xray_dir = sys.argv[1]
treenumber = pathlib.Path(xray_dir).parts[-1]

# get active view
renderView1 = GetActiveViewOrCreate("RenderView")

# Properties modified on renderView1
renderView1.UseColorPaletteForBackground = 0

# get the material library
materialLibrary1 = GetMaterialLibrary()

# Properties modified on renderView1
renderView1.Background = [1.0, 1.0, 1.0]

# Hide orientation axes
renderView1.OrientationAxesVisibility = 0

# create a new 'NetCDF Reader'
xraync = NetCDFReader(registrationName="xray.nc", FileName=[f"{xray_dir}/xray.nc"])

# show data in view
xrayncDisplay = Show(xraync, renderView1, "UniformGridRepresentation")

# trace defaults for the display properties.
xrayncDisplay.Representation = "Outline"

# reset view to fit data
renderView1.ResetCamera(False, 0.9)

# update the view to ensure updated data information
renderView1.Update()

# hide data in view
Hide(xraync, renderView1)

# create a new 'Contour'
contour1 = Contour(registrationName="Contour1", Input=xraync)


# show data in view
contour1Display = Show(contour1, renderView1, "GeometryRepresentation")

# trace defaults for the display properties.
contour1Display.Representation = "Surface"

# reset view to fit data
renderView1.ResetCamera(False, 0.9)
contour1.Isosurfaces = [950.0]

# show color bar/color legend
contour1Display.SetScalarBarVisibility(renderView1, True)

# update the view to ensure updated data information
renderView1.Update()

# get color transfer function/color map for 'data'
dataLUT = GetColorTransferFunction("data")

# get opacity transfer function/opacity map for 'data'
dataPWF = GetOpacityTransferFunction("data")

# get 2D transfer function for 'data'
dataTF2D = GetTransferFunction2D("data")

# turn off scalar coloring
ColorBy(contour1Display, None)

# Hide the scalar bar for this color map if no visible data is colored by it.
HideScalarBarIfNotNeeded(dataLUT, renderView1)

# create a new 'NetCDF Reader'
bilnc = NetCDFReader(registrationName="bil.nc", FileName=[f"{xray_dir}/bil.nc"])

# show data in view
bilncDisplay = Show(bilnc, renderView1, "UniformGridRepresentation")

# trace defaults for the display properties.
bilncDisplay.Representation = "Outline"

# update the view to ensure updated data information
renderView1.Update()

# create a new 'Transform'
transform1 = Transform(registrationName="Transform1", Input=bilnc)

# Properties modified on transform1.Transform
transform1.Transform.Translate = [-400.0, 0.0, 0.0]

# show data in view
transform1Display = Show(transform1, renderView1, "StructuredGridRepresentation")

# trace defaults for the display properties.
transform1Display.Representation = "Outline"

# hide data in view
Hide(bilnc, renderView1)

# update the view to ensure updated data information
renderView1.Update()

# create a new 'Contour'
contour2 = Contour(registrationName="Contour2", Input=transform1)

# show data in view
contour2Display = Show(contour2, renderView1, "GeometryRepresentation")

# trace defaults for the display properties.
contour2Display.Representation = "Surface"

# show color bar/color legend
contour2Display.SetScalarBarVisibility(renderView1, True)

# update the view to ensure updated data information
renderView1.Update()

# hide data in view
Hide(transform1, renderView1)

# turn off scalar coloring
ColorBy(contour2Display, None)

# Hide the scalar bar for this color map if no visible data is colored by it.
HideScalarBarIfNotNeeded(dataLUT, renderView1)

# ================================================================
# addendum: following script captures some of the application
# state to faithfully reproduce the visualization during playback
# ================================================================

# get layout
layout1 = GetLayout()

# --------------------------------
# saving layout sizes for layouts

# layout/tab size in pixels
layout1.SetSize(695, 909)

# -----------------------------------
# saving camera placements for views

# current camera placement for renderView1
renderView1.CameraPosition = [176.54338928363353, -2235.517103337426, 854.599164978424]
renderView1.CameraFocalPoint = [38.13334555795167, 112.86198528178713, 548.253544940588]
renderView1.CameraViewUp = [
    -0.017260080149817204,
    0.12833424422633485,
    0.991580763928021,
]
renderView1.CameraParallelScale = 753.4992643086075


##--------------------------------------------
## You may need to add some code at the end of this python script depending on your usage, eg:
#
## Render all views to see them appears
# RenderAllViews()
#
## Interact with the view, usefull when running from pvpython
# Interact()
#
## Save a screenshot of the active view
SaveScreenshot(f"/tmp/comparison/{treenumber}.png")
# SaveScreenshot("path/to/screenshot.png")
#
## Save a screenshot of a layout (multiple splitted view)
# SaveScreenshot("path/to/screenshot.png", GetLayout())
#
## Save all "Extractors" from the pipeline browser
# SaveExtracts()
#
## Save a animation of the current active view
# SaveAnimation()
#
## Please refer to the documentation of paraview.simple
## https://www.paraview.org/paraview-docs/latest/python/paraview.simple.html
##--------------------------------------------
```
