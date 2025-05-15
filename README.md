# Voice Cloning + Chatbot Demo (CS582 Final Project)

## Overview
This project combines:
- Whisper-based transcription
- GPT-2 simulation of an Ollama-style assistant
- Voice cloning via RVC (Retrieval-based Voice Conversion)

---

## Setup Instructions (Cross-Platform)

### 1. Clone the GitHub Repo
```bash
git clone https://github.com/your-team/voice-chatbot.git
cd voice-chatbot
```

### 2. Create a Virtual Environment (Recommended)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

---

## Required Assets (Google Drive)
Download these files from our shared [Google Drive folder](https://drive.google.com/drive/folders/1YIad0aTxlH1YVdtjwnRmabUeEZIOyVqC?usp=sharing):

| File                        | Destination Folder             |
|-----------------------------|--------------------------------|
| `myvoice_clean.wav`        | `dataset/myvoice/`             |
| `rmvpe.pt`                 | `assets/rmvpe/`                |
| `hubert_base.pt`           | `assets/hubert/`               |
| `logs/mi-test` (full dir)  | `logs/mi-test/`                |

Create any folders that don’t already exist (should already be existing).

---

## How to Run

### 1. Transcribe Voice File with Whisper
```bash
python whisper_transcribe.py
```

### 2. Chat with Transcription via GPT-2
```bash
python chatbot_response.py
```

---

## Course Connections (CS582)
This project demonstrates:
- Speech-to-text processing (Whisper → Lecture 10–11)
- Audio feature extraction and modeling (RVC → Lecture 14)
- Phoneme and pitch learning (RMVPE/Hubert → Lecture 3–4, 6)
- Sequence modeling via LLMs (GPT-2 simulation → Lecture 13)
- Applications of MFCCs, dynamic programming, and unsupervised learning for audio

---

## Team Members
- Lorenzo Ayala
- Ali Musa
- Mohamed Ali

Roles, versioning logs, and training notes tracked in the `/docs` folder.

---

## requirements.txt
```txt
openai-whisper
torch
transformers
scipy
sounddevice
numpy
```

---

## Notes
- No training is required to test the inference — all logs and checkpoints are provided.
- Compatible with Windows, macOS, and Linux (Python 3.10+ required for RVC stuff).


# [end of readme]
