# Sequence-to-Sequence Visual Question Answering (VQA)

This project focuses on building a sequence-to-sequence Visual Question Answering (VQA) model using deep learning techniques. It was developed as a midterm project for the Deep Learning course at Ton Duc Thang University.

## Project Description

The goal of this project is to create a VQA system that can answer questions based on an input image. The model combines a CNN for image feature extraction and an LSTM-based decoder for answer generation.

We experimented with:
- Using pretrained vs. non-pretrained CNN encoders (ResNet18).
- Using attention mechanism vs. no attention in the decoder.

## Features

- Detects transportation objects in images using YOLOv8.
- Automatically generates image-related questions and answers using Gemini API.
- Custom dataset creation with images, questions, and answers in JSON format.
- Sequence-to-sequence architecture with image-question encoder and LSTM decoder.
- Four experimental models with/without pretrained encoder and attention mechanism.
- Model evaluation with loss charts and real predictions.

## Model Architecture

### Encoder
- Pretrained ResNet18 for image feature extraction.
- LSTM for question encoding.
- Optional attention mechanism to merge image and question features.

### Decoder
- LSTM-based decoder to generate answer sequences.
- Trained using CrossEntropyLoss and Adam optimizer.
