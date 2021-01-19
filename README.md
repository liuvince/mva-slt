# Recvis - Topic F - Sign Language Translation from Video to Text

Vincent LIU liuvincent25@gmail.com

Supervised by Gül Varol

My code relies on the following repositories:

* https://github.com/neccam/slt [1]

* https://github.com/naver/dope [2]

## Compute DOPE [2] features on Phoenix14T Dataset [5]

![Dope.Viz](https://github.com/liuvince/mva-slt/blob/main/Slide/dope_viz.jpg)

## Early Fusion

![Early.Fusion](https://github.com/liuvince/mva-slt/blob/main/Slide/early_fusion.png)

Figure 1. Scheme of early fusion before projection and post projection (left) and a detailed overview of a single layered Sign LanguageTransformer (right) taken from [1]. The image example is from PHOENIX14T datatset [5].

## Late Fusion

![Late.Fusion](https://github.com/liuvince/mva-slt/blob/main/Slide/late_fusion.gif)

Equation 1. Equation of Late fusion.

## Code

Contains code to perform dope feature extraction, early-fusion and late-fusion.

## Features

```
https://drive.google.com/drive/folders/1Fc80pHwx8GNV4J-uzLENWD4i9r39RqO1
```

## Experiments

Contains the notebooks of my experiments.

## References

[1]  Necati  Cihan  Camgoz,  Oscar  Koller,  Simon  Hadfield,  and Richard Bowden.  Sign language transformers:  Joint end-to-end sign language recognition and translation, 2020.

[2]  Weinzaepfel, Philippe and Bregier, Romain and Combaluzier,Hadrien and Leroy, Vincent and Rogez, Gregory. DOPE: Distillation Of Part Experts for whole-body 3D pose estimation in the wild. In ECCV, 2020.

[3]  Necati Cihan Camgoz and Oscar Koller and Simon Hadfield and Richard Bowden.  Multi-channel Transformers for Multi-articulatory Sign Language Translation, 2020.

[4]  Oscar  Koller,  Necati  Camgoz,  Hermann  Ney,  and  Richard Bowden.  Weakly supervised learning with multi-stream cnn-lstm-hmms to discover sequential parallelism in sign language videos. IEEE Transactions on Pattern Analysis and Machine Intelligence, PP, 04 2019.

[5] Necati  Cihan  Camgoz,  Simon  Hadfield,  Oscar  Koller,  Hermann Ney, and Richard Bowden. Neural sign language translation.  InProceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), June 2018

