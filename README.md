# Conditioned-LSTM-Language-Model-for-Image-Captioning
Project from Natural Language Processing Course (COMS 4705) from Columbia University   
  
## Problem

Automatically generate natural language captions from images.

## Method

Implemented a conditioned LSTM image captioning model:

1. Images are encoded using a pretrained ResNet-18 CNN (final classification layer removed),
   producing 512-dimensional visual embeddings.

2. During decoding, each word embedding (512-d) is concatenated with the image embedding
   at every timestep, forming a 1024-d input to the LSTM.

3. The LSTM generates captions autoregressively, predicting one token at a time.

This architecture enables the language model to remain visually grounded throughout generation.

## Evaluation

Trained on Flickr8k and evaluated using BLEU scores.
Beam search was implemented to improve caption quality at inference.

Trained on Flicker dataset.

## Architecture

CNN → Feature Projection → LSTM → Softmax Vocabulary Output

## Tech Stack

- PyTorch
- ResNet
- LSTM
- MSCOCO

## Outcome

End-to-end multimodal deep learning system combining computer vision + NLP.
