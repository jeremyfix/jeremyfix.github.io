---
layout: page
permalink: /teaching/
title: teaching
description: Materials for courses I teach
nav: true
nav_order: 6
---

# Architecture des ordinateurs - CentraleSupelec (2025-)

This course deals with computer architecture, starting with the transitor and gradually building up the various layers of abstraction to finally reach programming. We’ll see the building blocks of information routing (multiplexer), memory (flip-flops, registers) and information processing (arithmetic and logic units) enabling the creation of data paths and their sequencing. The course ends with the programming of the architecture built in a language close to assembler and the realization of a mini-game, and ends by opening perspectives towards operating systems. All practical exercises will be carried out in Logisim simulation.

Full lecture is available on github [https://jeremyfix.github.io/Architecture/](https://jeremyfix.github.io/Architecture/)

**Illustration of the implemented architecture**

{% include video.liquid path="https://jeremyfix.github.io/Architecture/videos/archi-all.webm" title="Architecture running a sample code" class="video-fluid rounded z-depth-1" zoomable=true %}

# Python for scientists - CentraleSupelec (2025-)

The aim of this teaching unit is to train students in the tools of the Python ecosystem for scientists. It covers the use of specialized libraries for a number of major themes: scientific computing with Numpy, signal processing with Scipy, managing and processing large volumes of data with pandas, formatting results with matplotlib and an introduction to machine learning with scikit-learn.

Full lecture is available on github [https://jeremyfix.github.io/Python-for-scientists/](https://jeremyfix.github.io/Python-for-scientists/)

# Free softwares for engineers - CentraleSupelec (2025-)

This course introduces the main tools of the free software world useful to an engineer. It covers the use of bash to interact with the system, the philosophy behind GNU tools and how to combine them (pipelines, IO redirection, etc.). We’ll also take a look at how to combine various tools (git, python, awk, sed, lynx, ffmpeg, make), using them to carry out two projects. Assessment will be based on the practical reports.

Full lecture is available on github [https://jeremyfix.github.io/OutilsLibres/](https://jeremyfix.github.io/OutilsLibres/)

**Illustration of a video produced during the lecture**

{% include video.liquid path="https://youtu.be/tagmYHJ5Wxk" title="Mercury in front of the sun" %}

# Ingénierie Logicielle pour l'IA et la robotique - ILIAR - Université de Lorraine (2024 -)

The aim of this course is to design and implement a robotic system incorporating deep learning algorithms. It is structured around a central project involving the autonomous control of a simulated robot. Throughout the various sessions, students will learn how to:

- control the robot by sending motor commands,
- build an annotated learning base with these commands,
- train a convolutional neural network,
- deploy the trained network.

All of this is implemented using ROS2 middleware and the PyTorch library. This is a joint lecture with [Francis Colas](https://www.franciscolas.net/)

Full lecture is available on [https://ia2vr.gitlabpages.inria.fr/iliar/](https://ia2vr.gitlabpages.inria.fr/iliar/).

{% include video.liquid path="assets/video/iliar.webm" title="Autocontrol of a car with a neural network" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

# Deep learning - Master 2 IA2VR - Université de Lorraine (2024-)

This course is an introduction to deep learning. The full lecture materials is available on [https://ia2vr.gitlabpages.inria.fr/deeplearning](https://ia2vr.gitlabpages.inria.fr/deeplearning).

# Deep learning - CentraleSupélec - SDI-M (2024-2025)

## Lectures

- Lecture 1 [Introduction to deep learning and linear networks](https://frezza.pages.centralesupelec.fr/teachml2/Supports/NeuralNetworks/00-intro.html)
- Lecture 2 [Linear networks and RBF networks](https://frezza.pages.centralesupelec.fr/teachml2/Supports/NeuralNetworks/02-ffn.html)
- Lecture 3 [Convolutional Neural Networks](https://frezza.pages.centralesupelec.fr/teachml2/Supports/NeuralNetworks/03-cnn.html)
- Lecture 4 [Convolutional Neural Networks : Applications](https://frezza.pages.centralesupelec.fr/teachml2/Supports/NeuralNetworks/04-cnn.html)
- Lecture 5 [Recurrent Neural Networks and applications](https://frezza.pages.centralesupelec.fr/teachml2/Supports/NeuralNetworks/05-rnn.html)

## Labs

- Lab 1 [Introduction à pytorch](https://ia2vr.gitlabpages.inria.fr/iliar/pytorch_introduction.html)
- Lab 2 [Segmentation sémantique avec un modèle encodeur/décodeur sur Pascal-VOC](https://ia2vr.gitlabpages.inria.fr/deeplearning/lab2.html)
- Lab 3 [Automatic Speech Recognition](https://teaching.pages.centralesupelec.fr/deeplearning-lectures-build/02-pytorch-asr.html)
- Lab 4 [Deep Convolutional Generative Adversarial Networks](https://teaching.pages.centralesupelec.fr/deeplearning-lectures-build/03-pytorch-gan.html)

## Challenges

- 2024-2025 [Zooplankton semantic segmentation](https://www.kaggle.com/competitions/3md4040-2025-challenge/overview)

To have an idea about the performances of the teams, below are renderings of the
predictions on the test images where the color code is :

- blue: true negatives
- green : true positives
- red : false positives
- purple: false negatives

<div class="row">
	<div class="col-sm-2">
	🥱 F1=0.926
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/1_polaih63_jurand_maxdodo_durand/pred_rg20090121_mask.png" title="Team 1, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/1_polaih63_jurand_maxdodo_durand/pred_rg20090520_mask.png" title="Team 1, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	C'est lui ☝️, F1=0.92364
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/2_vanderbeken/pred_rg20090121_mask.png" title="Team 2, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/2_vanderbeken/pred_rg20090520_mask.png" title="Team 2, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	AST, F1=0.91470
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/3_xavelche_sultan_bertho_pelhate/pred_rg20090121_mask.png" title="Team 3, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/3_xavelche_sultan_bertho_pelhate/pred_rg20090520_mask.png" title="Team 3, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	العبرة بالخواتيم, F1=0.91287
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/4_echaabi_mockbel_hard_talaa/pred_rg20090121_mask.png" title="Team 4, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/4_echaabi_mockbel_hard_talaa/pred_rg20090520_mask.png" title="Team 4, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	Random predictions 2, F1=0.91151
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/5_plisson_manuelito_blondel_leveugle/pred_rg20090121_mask.png" title="Team 5, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/5_plisson_manuelito_blondel_leveugle/pred_rg20090520_mask.png" title="Team 5, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	Huguo Bui, F1=0.90933
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/6_gomes_aka_bui_alexialan/pred_rg20090121_mask.png" title="Team 6, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/6_gomes_aka_bui_alexialan/pred_rg20090520_mask.png" title="Team 6, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	C'est qui l'patron ? 🙄, F1=0.90897
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/7_fix/pred_rg20090121_mask.png" title="Team 7, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/7_fix/pred_rg20090520_mask.png" title="Team 7, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	Eliott, F1=0.90218
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/8_dumont_merjani/pred_rg20090121_mask.png" title="Team 8, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/8_dumont_merjani/pred_rg20090520_mask.png" title="Team 8, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	., F1=0.90061
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/9_yvan_malick_dhaou_diallo/pred_rg20090121_mask.png" title="Team 9, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/9_yvan_malick_dhaou_diallo/pred_rg20090520_mask.png" title="Team 9, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	100% Homemade UNet, F1=0.88907
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/10_capitant_malloi_theo_moine/pred_rg20090121_mask.png" title="Team 10, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/10_capitant_malloi_theo_moine/pred_rg20090520_mask.png" title="Team 10, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	TN, F1=0.88580
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/11_yesmine_bouattour_abbes_rayen/pred_rg20090121_mask.png" title="Team 11, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/11_yesmine_bouattour_abbes_rayen/pred_rg20090520_mask.png" title="Team 11, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	Still in the bottom, F1=0.86602
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/12_haris/pred_rg20090121_mask.png" title="Team 12, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/12_haris/pred_rg20090520_mask.png" title="Team 12, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	Wassim Behlaj, F1=0.85713
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/13_belhaj/pred_rg20090121_mask.png" title="Team 13, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/13_belhaj/pred_rg20090520_mask.png" title="Team 13, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="row">
	<div class="col-sm-2">
	Etienne Andrier, F1=0.83777
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/14_andrier/pred_rg20090121_mask.png" title="Team 14, first image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2024_deep_challenge/14_andrier/pred_rg20090520_mask.png" title="Team 14, second image" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>

- 2023-2024 : we participated to the [GeoLifeClef 2022 challenge](https://www.kaggle.com/competitions/geolifeclef-2022-lifeclef-2022-fgvc9/overview), after the competition was over. The final leaderboard of the teams is shown below.

<div class="row">
    <div class="col-sm-4">
	</div>
    <div class="col-sm-4">
		{% include figure.liquid path="assets/img/2022_2023_leaderboard.png" title="2022-2023 Leaderboard" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4">
	</div>
</div>

- 2022-2023 [Phytoplankton temporal series prediction](https://www.kaggle.com/c/temporal-prediction-of-plankton)
- 2021-2022 [Zooplankton classification](https://www.kaggle.com/c/3md4040-2022-challenge)
