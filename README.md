# YouTube Downloader & AI Summary Generator

This project allows you to:
1. Download YouTube videos.
2. Extract and upload audio to Google Cloud Storage.
3. Transcribe speech using **Google Cloud Speech-to-Text**.
4. Generate summaries using **Google Gemini**.
5. Interact via a **Gradio web interface** with a video preview feature.

---

## **Features**
- **YouTube Video Download** using `yt-dlp`.
- **Audio Extraction & Conversion** with `pydub` (FFmpeg required).
- **Google Cloud Integration** for:
  - Speech-to-Text transcription.
  - Storage bucket upload.
- **AI Summary Generation** using **Google Gemini** (`google-genai`).
- **Gradio Web UI** for an easy-to-use interface.

---

## **Requirements**
- Python 3.9+
- Google Cloud Project with:
  - Speech-to-Text API enabled
  - Cloud Storage enabled
- Gemini API key or Vertex AI setup
- FFmpeg installed

---

## **Setup**
1. **Clone the repository**
   ```bash
   git clone https://github.com/Ayush0135/youtube-downloader-ai.git
   cd youtube-downloader-ai


   export GOOGLE_APPLICATION_CREDENTIALS="/path/to/your-service-account.json"
export GCS_BUCKET_NAME="your-bucket-name"
export GEMINI_API_KEY="your-gemini-api-key"

Usage
Paste a YouTube link in the Gradio interface.


The app will:

Download the video.

Extract audio and upload to GCS.

Transcribe speech.

Summarize content using Gemini.

Display results in the browser.
