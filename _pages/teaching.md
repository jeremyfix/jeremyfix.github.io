---
layout: page
permalink: /teaching/
title: teaching
description: Materials for courses I teach
nav: true
nav_order: 6
---

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

- 2024-2025 [Zooplankton semantic segmenation](https://www.kaggle.com/competitions/3md4040-2025-challenge/overview)

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
