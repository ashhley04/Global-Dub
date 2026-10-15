# 🌍 Global Dub — AI-Powered Multilingual Video Dubbing

**Breaking language barriers through AI-powered video translation and dubbing.**

Global Dub is an AI-powered multilingual video dubbing application designed to make video content more accessible to people across India. It transforms English-language videos into dubbed versions in Indian regional languages, helping viewers understand educational content, motivational videos, and other media in their preferred language.

The application combines automatic speech recognition, machine translation, text-to-speech synthesis, and video processing to automate the dubbing workflow.

## ✨ Features

- **🎙️ Speech Recognition:** Uses OpenAI Whisper to extract spoken content from uploaded videos.
- **🌐 Multilingual Translation:** Translates transcribed English speech into the selected Indian regional language using Google Translate.
- **🗣️ AI Voice Generation:** Uses Google Text-to-Speech (gTTS) to generate dubbed audio in the target language.
- **🎬 Video Processing:** Integrates the generated audio into the original video using MoviePy.
- **🇮🇳 Indian Language Support:** Supports multiple languages to improve accessibility for diverse linguistic communities.
- **📥 Video Upload and Download:** Allows users to upload videos through a web interface and download the processed output.
- **🖥️ Web-Based Interface:** Built with Flask, HTML, and CSS for a simple user experience.

## 🗣️ Supported Languages

The application currently supports the following target languages:

| Language | Language Code |
|---|---|
| English | `en` |
| Hindi | `hi` |
| Malayalam | `ml` |
| Marathi | `mr` |
| Tamil | `ta` |
| Gujarati | `gu` |
| Telugu | `te` |
| Kannada | `kn` |

## ⚙️ Technology Stack

- **Programming Language:** Python
- **Web Framework:** Flask
- **Speech Recognition:** OpenAI Whisper
- **Machine Translation:** Google Translate (`googletrans`)
- **Text-to-Speech:** Google Text-to-Speech (`gTTS`)
- **Video and Audio Processing:** MoviePy
- **Data and File Handling:** JSON and Python file-processing utilities
- **Frontend:** HTML, CSS
- **Development Tools:** VS Code / PyCharm

## 🔄 How It Works

1. **Upload Video:** The user uploads an English-language video through the web application.
2. **Extract Speech:** OpenAI Whisper transcribes the speech from the video into text.
3. **Translate Text:** Google Translate converts the transcription into the selected target language.
4. **Generate Dubbed Audio:** gTTS converts the translated text into speech in the target language.
5. **Replace Audio Track:** MoviePy integrates the generated audio with the original video.
6. **Download Output:** The application returns the processed video for the user to download.

### Workflow

`English Video` → `Whisper Transcription` → `Google Translate` → `gTTS Voice Generation` → `MoviePy Audio Integration` → `Dubbed Video`

## 🚀 Getting Started

### Prerequisites

Ensure that you have the following installed:

- Python 3.9 (or another compatible Python version)
- pip
- FFmpeg, if required by your MoviePy installation
- Git

The application also requires an internet connection for services such as Google Translate and gTTS.

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Global-Dub
```

Replace `<YOUR_GITHUB_REPOSITORY_URL>` with your actual GitHub repository URL.

### 2. Create a Virtual Environment

**Windows PowerShell:**

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, you can activate the environment from Command Prompt instead:

```cmd
venv\Scripts\activate.bat
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If the existing dependency file causes installation errors, check the Python version and package compatibility before updating the dependencies.

### 4. Run the Application

```bash
python main.py
```

Open the following URL in your browser:

```text
http://127.0.0.1:5907
```

Upload a supported video, select a target language, and submit it for processing.

## 📁 Project Structure

```text
Global-Dub/
│
├── main.py                  # Flask application and dubbing pipeline
├── requirements.txt         # Python dependencies
├── package.json             # Node.js package metadata
│
├── templates/
│   ├── index.html           # Homepage
│   ├── upload.html          # Video upload interface
│   └── thankyou.html        # Thank-you page
│
└── static/
    ├── styles.css           # Frontend styling
    ├── *.png                # Interface assets and icons
    ├── *.jpg                # Language and interface images
    └── *.mp4                # Sample and output video assets
```

*Note: The `static` directory may contain sample videos and generated output files. The exact contents can vary depending on the version of the project.*

## 🎯 Problem Statement

India has a diverse linguistic landscape, and useful video content is not always accessible to people who are less comfortable with English. Language barriers can limit access to educational resources, motivational content, and information available online.

Global Dub addresses this challenge by automating the core stages of video dubbing, enabling English-language content to be converted into selected Indian regional languages through a web-based application.

## 💡 Applications

- Regional-language educational content
- Multilingual motivational videos
- Language accessibility for online media
- Localization of digital video content
- Wider distribution of informational content across linguistic communities

## ⚠️ Limitations

- The current implementation primarily assumes that the source speech is in English.
- Translation accuracy depends on the transcription and machine translation services.
- Generated speech may not match the original speaker's voice, tone, or speaking pace.
- The implementation replaces the original audio track; synchronized lip movements are not generated.
- Processing time depends on video duration, available computing resources, and external service response times.
- Internet access is required for Whisper model downloads when not already cached, as well as online translation and text-to-speech services.

## 🔮 Future Enhancements

- Support for automatic source-language detection and multilingual input.
- Better alignment of generated speech with the original video duration.
- Subtitle generation and downloadable translated transcripts.
- Improved voice quality and speaker-preserving dubbing.
- More Indian regional languages.
- Improved error handling, temporary file management, and secure upload validation.
- Deployment as a scalable web application.

## 👩‍💻 Project Objective

Global Dub demonstrates how AI and software development can be combined to build a practical multilingual media solution. By integrating speech recognition, machine translation, text-to-speech, and video processing, the project explores ways to make digital content more inclusive and accessible to India's diverse linguistic communities.

---

**Built with Python, Flask, Whisper, Google Translate, gTTS, and MoviePy.**
