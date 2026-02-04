# Conditioned-LSTM-Language-Model-for-Image-Captioning
Project from Natural Language Processing Course (COMS 4705) from Columbia University   
  
## Problem

Automatically generate natural language captions from images.

## Method

Pipeline:

1. Pretrained CNN extracts visual features
2. Feature vectors condition an LSTM language model
3. LSTM generates word sequences autoregressively

Trained on Flicker dataset.

## Evaluation

Performance measured using BLEU scores.

Model successfully learned visual-language alignment and produced semantically coherent captions.

## Architecture

CNN → Feature Projection → LSTM → Softmax Vocabulary Output

## Tech Stack

- PyTorch
- ResNet
- LSTM
- MSCOCO

## Outcome

End-to-end multimodal deep learning system combining computer vision + NLP.
