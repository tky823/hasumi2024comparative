---
title: A COMPARATIVE STUDY OF TEXT-SPEECH ALIGNMENT METHODS FOR EMOTIONAL SPEECH SYNTHESIS
layout: default
---

# Authors

<div style="text-align: center;">
Anonymous submission to Interspeech 2024
</div>

# Abstract

In this paper, we investigate the performance of various text-speech alignment methods to build a high-quality emotional parallel text-to-speech (TTS) system.
We not only make a comprehensive study on text-speech alignment strategies on emotional TTS tasks but also propose a semi-supervised alignment learning approach as an extension of unsupervised alignment learning.
In the semi-supervised approach, the alignment module is pre-trained with a small amount of annotated data and then fine-tuned with a large amount of unannotated data.
The main findings from experimental results include that the semi-supervised approach, which uses only 4% of annotated data, significantly improves the training stability of the unsupervised approach.
Moreover, it achieves comparable performance to a model that employs fully annotated duration labels and the alignments extracted from a strong external forced aligner.

# Audio Samples

## Neutral Style

| Model | Sample 1 (Female) | Sample 2 (Male) |
|:-:|:-:|:-:|
| Reference | <audio controls src="samples/Reference/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Reference/neutral/mksk04983.wav"></audio> |
| Period-VITS (manual) | <audio controls src="samples/Period-VITS_manual/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Period-VITS_manual/neutral/mksk04983.wav"></audio> |
| Period-VITS (external) | <audio controls src="samples/Period-VITS_external/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Period-VITS_external/neutral/mksk04983.wav"></audio> |
| Semi-Period-VITS | <audio controls src="samples/Semi-RAD-Period-VITS/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Semi-RAD-Period-VITS/neutral/mksk04983.wav"></audio> |
| Un-Period-VITS | <audio controls src="samples/RAD-Period-VITS/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/RAD-Period-VITS/neutral/mksk04983.wav"></audio> |

## Happiness Style

| Model | Sample 1 (Female) | Sample 2 (Male) |
|:-:|:-:|:-:|
| Reference | <audio controls src="samples/Reference/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Reference/happy/mksk41204.wav"></audio> |
| Period-VITS (manual) | <audio controls src="samples/Period-VITS_manual/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Period-VITS_manual/happy/mksk41204.wav"></audio> |
| Period-VITS (external) | <audio controls src="samples/Period-VITS_external/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Period-VITS_external/happy/mksk41204.wav"></audio> |
| Semi-Period-VITS | <audio controls src="samples/Semi-RAD-Period-VITS/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Semi-RAD-Period-VITS/happy/mksk41204.wav"></audio> |
| Un-Period-VITS | <audio controls src="samples/RAD-Period-VITS/happy/fkdo41271.wav"></audio> | <audio controls src="samples/RAD-Period-VITS/happy/mksk41204.wav"></audio> |

## Sadness Style

| Model | Sample 1 (Female) | Sample 2 (Male) |
|:-:|:-:|:-:|
| Reference | <audio controls src="samples/Reference/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Reference/sad/mksk51196.wav"></audio> |
| Period-VITS (manual) | <audio controls src="samples/Period-VITS_manual/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Period-VITS_manual/sad/mksk51196.wav"></audio> |
| Period-VITS (external) | <audio controls src="samples/Period-VITS_external/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Period-VITS_external/sad/mksk51196.wav"></audio> |
| Semi-Period-VITS | <audio controls src="samples/Semi-RAD-Period-VITS/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Semi-RAD-Period-VITS/sad/mksk51196.wav"></audio> |
| Un-Period-VITS | <audio controls src="samples/RAD-Period-VITS/sad/fkdo51172.wav"></audio> | <audio controls src="samples/RAD-Period-VITS/sad/mksk51196.wav"></audio> |

# References

- [1] Y. Shirahata, et al., "Period VITS: Variational inference with explicit pitch modeling for end-to-end emotional speech synthesis," in *Proc. ICASSP*, 2023, pp.1-5.
- [2] K. J. Shih, et al., "RAD-TTS: Parallel frlo-based TTS with robust alignment learning and diverse synthesis.", in *ICML workshop*, 2021.
