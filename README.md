# 📝 Grammar Scoring Engine for Voice Samples

This repository contains a Jupyter Notebook that demonstrates a complete pipeline to score spoken English grammar from audio samples using a deep learning approach. The model listens to an audio clip, transcribes it, and then evaluates the grammar accuracy of the spoken content by predicting a score between 0 and 5.

## 🚀 Overview

The goal is to build a model that:
- Takes an audio file as input
- Transcribes the audio into text using OpenAI's Whisper
- Scores the grammatical quality of the transcribed text using a fine-tuned DeBERTa model

## 📂 Dataset

The dataset consists of:
- **Audio files** in `.wav` format (45–60 seconds)
- **train.csv** — contains filenames and corresponding grammar scores (1–5)
- **test.csv** — contains filenames with placeholder labels
- **sample_submission.csv** — sample format for your predictions

Grammar scores are based on the MOS Likert scale, with `1` indicating poor grammar and `5` representing excellent grammatical fluency.
