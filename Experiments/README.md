Table 1. Baseline:  Results trying to reproduce Table 4 from [1].Training SLT to jointly learn recognition and translation with different weight on recognition loss with baseline features obtained from [4].

| Recognition Loss Weights | DEV WER | DEV BLEU-4 | TEST WER | TEST BLEU-4 
| --- | --- | --- | --- | --- |
| 0.0 | - | 18.75 | - | 18.92 | 
| 1.0 | 41.53 | **21.08** | 41.11 | 20.41 |
| 2.5 | 31.71 | 20.40 | 31.32 | 19.79 |
| 5.0 | **28.82** | 19.39 | **28.55** | 20.49 |
| 10.0 | 30.48 | 20.18 | 29.96 | 19.86 |
| 20.0 | 30.61 | 19.80 | 31.30 | 20.52 |
| 40.0 | 32.53 | 20.32 | 32.50 | **20.64** |

Table 2. Early Fusion: Training SLT [1] by adding single articula-tory keypoint coordinates to theBaseline features [4], with different combination of loss weights. Measurement metric is BLEU-4on TEST set.

| Input | Loss recognition weights | 2D | 3D |
| --- | --- | --- | --- | 
| Baseline | 40.0 | **20.64** | 20.64 |
| B + hands | 1.0 | 19.23 | 20.66 |
| B + hands | 20.0 | 20.60 | 19.40 |
| B + hands | 40.0 | 19.20 | **20.72** |
| B + body | 1.0 | 20.13 | 18.83 |
| B + body | 20.0 | 19.40 | **20.87** |
| B + body | 40.0 | 19.43 | 20.51 |
| B + face | 1.0 | 18.50 | **20.54** |
| B + face | 20.0 | 20.45 | 20.03 |
| B + face | 40.0 | 19.63 | 20.29 |

Table 3. Early Fusion: Training SLT [1] by adding multiple articulately cues (Keypoints coordinates,Hidden features from [2]) to the Baseline features [4] for different combination of loss weights.

| Input | Recognition Loss Weights | DEV WER | DEV BLEU-4 | TEST WER | TEST BLEU-4 
| --- | --- | --- | --- | --- | --- |
| B | 40.0 | 32.53 | 20.32 | 32.50 | **20.64** |
| B + K | 1.0 | 49.64 | 20.08 | 48.09 | 19.58 |
| B + K | 20.0 | 32.05 | 19.72 | 32.43 | 20.05 |
| B + K | 40.0 | 28.32 |**20.76** | 29.21 | 20.19 |
| B + H | 1.0 | 46.41 | 20.16 | 45.50 | 19.67 |
| B + H | 20.0 | **27.89** | 19.89 | **28.39** | 19.79 |
| B + H | 40.0 | 29.44 | 20.20 | 29.21| 20.55 |
| B + K + H | 1.0 | 43.88 | 19.84 | 43.51 | 19.84 |
| B + K + H | 20.0 | 28.82 | 20.62 | 29.04 | **20.81** |
| B + K + H | 40.0 | 30.85 | 19.91 | 30.66 | 19.44 |

Table 4. Early Fusion post projection: Training SLT [1] by addingmultiple articulately cues (Keypoints coordinates,Hidden featuresfrom [2]) to theBaseline features [4] for different combination ofloss weights

| Input | Recognition Loss Weights | DEV WER | DEV BLEU-4 | TEST WER | TEST BLEU-4 
| --- | --- | --- | --- | --- | --- |
| B | 40.0 | **32.53** | **20.32** | **32.50** | **20.64** |
| B + K | 1.0 | 37.02 | 18.70 | 36.60 | 19.17 |
| B + K | 20.0 | 34.67 | 18.98 | 34.89 | 18.59 |
| B + K | 40.0 | 39.34 | 19.42 | 39.14 | 19.29 |
| B + H | 1.0 | 39.34 | 19.62 | 39.73 | 18.68 |
| B + H | 20.0 | 37.87 | 19.61 | 34.28 | 19.42 |
| B + H | 40.0 | 47.32 | 18.51 | 46.04 | 18.48 |
| B + K + H | 1.0 | 39.93 | 19.56 | 39.77 | 19.26 |
| B + K + H | 20.0 | 33.33 | 19.75 | 33.74 | 19.96 |
| B + K + H | 40.0 | 38.00 | 18.18 | 37.47 | 19.96 |

Table 5. Baseline for late fusion: Training SLT [1] with only dope outputs [2] as input, with different combination of loss weights.

| Input | Loss recognition weights | DEV | TEST |
| --- | --- | --- | --- | 
| Baseline | 40.0 | **20.64** | **20.64** |
| K | 1.0 | 10.21 | 10.21 |
| K | 20.0 | 11.82 | 11.49 |
| K | 40.0 | 11.84 | **12.04** |
| H | 1.0 | 13.50 | 13.11 |
| H | 20.0 | 16.20 | 15.17 |
| H | 40.0 | 15.51 | **15.58** |

Table 6. Late Fusion:  Predicting SLT [1] by averaging the class probabilities between different small models

| Input | Recognition Loss Weights | DEV WER | DEV BLEU-4 | TEST WER | TEST BLEU-4 
| --- | --- | --- | --- | --- | --- |
| B | 40.0 | **32.53** | 20.32 | **32.50** | 20.64 |
| B + K | 1.0 | 54.68 | 19.49 | 53.60 | 19.01 |
| B + K | 20.0 | 46.25 | 19.36 | 46.58 | 19.23 |
| B + K | 40.0 | 47.56 | 19.64 | 47.45 | 19.81 |
| B + H | 1.0 | 52.60 | 21.08 | 51.02 | 20.05 |
| B + H | 20.0 | 51.19 | 20.42 | 50.72 | 20.15 |
| B + H | 40.0 | 49.76 | **20.84** | 47.90 | **21.51** |
| B + K + H | 1.0 | 61.01 | 20.30 | 59.29 | 19.73 |
| B + K + H | 20.0 | 58.47 | 20.35 | 57.38 | 20.11 |
| B + K + H | 40.0 | 59.33 | 20.61 | 58.23 | 21.24 |


# References

[1]  Necati  Cihan  Camgoz,  Oscar  Koller,  Simon  Hadfield,  and Richard Bowden.  Sign language transformers:  Joint end-to-end sign language recognition and translation, 2020.
[2]  Weinzaepfel, Philippe and Bregier, Romain and Combaluzier,Hadrien and Leroy, Vincent and Rogez, Gregory. DOPE: Distillation Of Part Experts for whole-body 3D pose estimation in the wild. In ECCV, 2020.
[3]  Necati Cihan Camgoz and Oscar Koller and Simon Hadfield and Richard Bowden.  Multi-channel Transformers for Multi-articulatory Sign Language Translation, 2020.
[4]  Oscar  Koller,  Necati  Camgoz,  Hermann  Ney,  and  Richard Bowden.  Weakly supervised learning with multi-stream cnn-lstm-hmms to discover sequential parallelism in sign language videos. IEEE Transactions on Pattern Analysis and Machine Intelligence, PP, 04 2019.
[5] Necati  Cihan  Camgoz,  Simon  Hadfield,  Oscar  Koller,  Hermann Ney, and Richard Bowden. Neural sign language translation.  InProceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), June 2018




