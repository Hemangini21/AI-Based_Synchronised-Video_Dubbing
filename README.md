

# 🎙️ SYNCVOX:AI-Based Synchronized Video Dubbing

An AI-powered system that dubs videos into multiple languages while preserving **lip-sync**, **emotion**, and **voice consistency**. It automates the process using advanced ASR, translation, emotional TTS, and Wav2Lip for realistic synchronization.

---

## 📁 Project Structure

```
AI-Based_Synchronised-Video_Dubbing/
│
├── backend/          # Core AI components (ASR, TTS, Wav2Lip, etc.)
├── flask-api/        # Flask API backend to serve AI services
├── frontend/         # UI for uploading videos and selecting language/emotion
└── README.md         # Project documentation
```

---

## ⚙️ How It Works

```mermaid
graph TD
A[🎥 Input Video] --> B[🧠 ASR (Speech-to-Text)]
B --> C[🌐 Translation (MarianMT)]
C --> D[🗣️ Emotional TTS (FastSpeech 2)]
D --> E[👄 Lip Sync with Wav2Lip]
E --> F[📼 Render Dubbing Output]
```

> The system breaks down input videos, transcribes speech, translates it, generates emotional speech, syncs lips to the new voice, and re-renders the video — all automatically.

---

## 🔧 Tech Stack

| Layer      | Technology                           |
|------------|---------------------------------------|
| Frontend   | React+ Vite      |
| API Layer  | Flask (Python REST API)               |
| Backend    | PyTorch, OpenCV, FFmpeg               |
| AI Models  | Whisper, GTTS, FastSpeech2, Wav2Lip |

---
## 🧪 Output Video


## 📚 References

- [Wav2Lip (CVPR 2020)](https://github.com/Rudrabha/Wav2Lip)  
- [FastSpeech 2 (Microsoft Research)](https://arxiv.org/abs/2006.04558)  
- [Whisper by OpenAI](https://github.com/openai/whisper)  
