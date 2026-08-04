# 🎙️ Hindi ASR Pipeline: Whisper-Small Fine-Tuning

An end-to-end Automatic Speech Recognition (ASR) pipeline for Hindi using OpenAI's **Whisper-Small** model. This project covers dataset preprocessing, model fine-tuning, evaluation, Word Error Rate (WER) comparison, and systematic error analysis.

---

## 📌 Project Overview

This project was developed to fine-tune Whisper-Small for Hindi speech recognition and compare its performance against the pretrained model.

The workflow includes:

- Audio preprocessing
- Dataset cleaning
- Whisper-Small fine-tuning
- Evaluation on the Hindi portion of the FLEURS dataset
- Word Error Rate (WER) comparison
- Error analysis and taxonomy
- Recommendations for improving ASR performance

---

## 🚀 Objectives

- Prepare the Hindi speech dataset for training.
- Fine-tune Whisper-Small.
- Evaluate both pretrained and fine-tuned models.
- Report Word Error Rate (WER).
- Analyze transcription errors.
- Categorize common error types.
- Propose improvements based on observed errors.

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `cleanup_pipeline.ipynb` | Dataset preprocessing and cleaning pipeline |
| `pretrained_whisper_AsrData.ipynb` | Baseline evaluation using pretrained Whisper-Small |
| `fine_tuned_whisper_Evaluation.ipynb` | Evaluation of the fine-tuned Whisper model |
| `pretrained_whispersmall_Evaluation.ipynb` | Performance comparison of pretrained model |
| `Question_1.ipynb` | Dataset preprocessing and preparation |
| `question3.ipynb` | Error analysis and taxonomy |
| `dataset.jsonl` | Processed training dataset |
| `tagged_asr.csv` | Error-tagged ASR predictions |
| `final_word_labels.csv` | Word-level annotations |
| `FT Data - Google Sheets.pdf` | Supporting documentation and analysis |

---

# Dataset Preprocessing

The preprocessing pipeline includes:

- Audio validation
- Removal of corrupted samples
- Missing transcript handling
- Audio resampling to **16 kHz**
- Feature extraction
- Transcript normalization
- Dataset formatting for Whisper training

---

# Model

- Base Model: **OpenAI Whisper-Small**
- Framework: Hugging Face Transformers
- Task: Hindi Automatic Speech Recognition

---

# Fine-Tuning Pipeline

The model training consists of:

1. Data preprocessing
2. Audio feature extraction
3. Tokenization
4. Whisper-Small fine-tuning
5. Model evaluation

---

# Evaluation

The pretrained and fine-tuned Whisper-Small models are evaluated on the **Hindi subset of the FLEURS test dataset**.

Evaluation metric:

- Word Error Rate (WER)

---

# Results

| Model | WER |
|--------|----:|
| Pretrained Whisper-Small | XX.XX% |
| Fine-Tuned Whisper-Small | XX.XX% |

> Replace with your experimental results.

---

# Error Analysis

A systematic analysis was conducted on at least **25 incorrectly transcribed utterances**.

Each error contains:

- Reference transcript
- Predicted transcript
- Error category
- Root cause

---

# Error Taxonomy

The observed transcription errors were grouped into categories such as:

- Word substitution
- Word deletion
- Word insertion
- Named entity errors
- Numeral recognition errors
- Homophone confusion
- Noise-induced transcription errors
- Pronunciation variation

---

# Proposed Improvements

Based on the most frequent errors:

- Improve transcript normalization
- Add pronunciation-diverse training samples
- Apply noise augmentation
- Optimize decoding parameters
- Domain-specific fine-tuning
- Language model-assisted decoding

---

# Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Whisper
- Torchaudio
- Librosa
- Pandas
- NumPy
- Matplotlib

---

# How to Run

1. Clone the repository

```bash
git clone https://github.com/<your-username>/Hindi-ASR-Pipeline-Whisper-small-Fine-tuning.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the notebooks in order:

- cleanup_pipeline.ipynb
- Question_1.ipynb
- pretrained_whisper_AsrData.ipynb
- pretrained_whispersmall_Evaluation.ipynb
- fine_tuned_whisper_Evaluation.ipynb
- question3.ipynb

---

# Future Work

- Train on larger Hindi speech corpora
- Experiment with Whisper-Medium and Whisper-Large
- Improve decoding strategies
- Real-time Hindi ASR deployment
- Speaker adaptation

---

# Author

**Mohit Raj**

B.Tech (Hons.) in Data Science

Machine Learning • Deep Learning • Speech Processing • Generative AI

---
