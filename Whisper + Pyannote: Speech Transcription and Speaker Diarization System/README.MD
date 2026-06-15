# 🎙️ Whisper + Pyannote: Speech Transcription and Speaker Diarization System

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MohamedElsagheer95/llm-engineering/blob/main/%20%20%20%20llm-engineering%20%20/Whisper%20%2B%20Pyannote%3A%20Speech%20Transcription%20and%20Speaker%20Diarization%20System/Whisper%2BPyannote(speach_recognition_and_diarization).ipynb)

This project provides a complete pipeline for **automatic speech recognition (ASR)** and **speaker diarization** using state‑of‑the‑art models:

- **Transcription** – [Faster‑Whisper](https://github.com/SYSTRAN/faster-whisper) (large‑v3) for fast and accurate speech‑to‑text.
- **Diarization** – [Pyannote](https://github.com/pyannote/pyannote-audio) (speaker‑diarization‑3.1) to identify who spoke and when.
- **Audio preprocessing** – FFmpeg for mono conversion, band‑pass filtering, and noise reduction.
- **Output** – Combined transcript with speaker labels and timestamps, plus an SRT subtitle file.

The notebook is designed to run on **Google Colab** with GPU acceleration (T4 recommended). It works especially well for **Arabic** speech (tested on an Arabic conversation), but can be adapted to other languages.

---

## 📋 Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Output Format](#output-format)
- [Customisation](#customisation)
- [Acknowledgements](#acknowledgements)
- [License](#license)

---

## ✨ Features

- ✅ **High‑quality transcription** – Faster‑Whisper large‑v3 with VAD (Voice Activity Detection)
- ✅ **Speaker diarisation** – Identifies up to 8 speakers, assigns labels (SPEAKER_01, etc.)
- ✅ **Audio preprocessing** – Converts to mono (16 kHz), applies high‑pass (120 Hz) / low‑pass (3800 Hz) filters, and basic noise reduction
- ✅ **Time‑aligned output** – Merges transcription segments with the most likely speaker using overlap scoring
- ✅ **Subtitle generation** – Saves a standard `.srt` file from the transcript
- ✅ **GPU optimised** – Runs on CUDA with `float16` for speed

---

## 🧰 Prerequisites

- A **Google account** to run the Colab notebook (or local machine with NVIDIA GPU)
- **Hugging Face account** and a **User Access Token** (for Pyannote model)
  - Accept the terms of use for [pyannote/speaker-diarization-3.1](https://huggingface.co/pyannote/speaker-diarization-3.1)
- Input audio file (MP3, WAV, etc.) – the notebook uses `/content/bakar1.mp3` as an example

---

## 🚀 Installation & Setup

### 1. Open the Notebook in Colab

Click the **Open In Colab** badge at the top of this README or go directly to the [notebook link](https://colab.research.google.com/github/MohamedElsagheer95/llm-engineering/blob/main/%20%20%20%20llm-engineering%20%20/Whisper%20%2B%20Pyannote%3A%20Speech%20Transcription%20and%20Speaker%20Diarization%20System/Whisper%2BPyannote(speach_recognition_and_diarization).ipynb).

### 2. Install Dependencies

Run the first code cell to install required libraries:

```bash
pip install faster-whisper pyannote.audio torch transformers
