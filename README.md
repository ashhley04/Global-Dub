# 🌍 Global Dub — AI-Powered Multilingual Video Dubbing

**Breaking language barriers through AI-powered video translation and dubbing.**

Global Dub is an AI-powered multilingual video dubbing application designed to make video content more accessible to people across India. It converts English-language videos into dubbed versions in Indian regional languages, helping viewers access educational content, motivational videos, and other media in their preferred language.

The application integrates automatic speech recognition, machine translation, text-to-speech synthesis, and video processing to automate the video dubbing workflow.

## 🎥 Project Demo

Watch Global Dub in action and explore how AI can help make video content accessible across different Indian regional languages.

**▶️ [Click here to watch the Global Dub Demo](https://youtu.be/Z64pYDqK7S8)**

<!-- Replace YOUR_VIDEO_LINK_HERE with your YouTube demo URL or other accessible video link. -->

## ✨ Features

- 🎙️ **Speech Recognition:** Uses OpenAI Whisper to transcribe spoken content from uploaded videos.
- 🌐 **Multilingual Translation:** Translates transcribed English speech into the selected Indian regional language using Google Translate.
- 🗣️ **Text-to-Speech Synthesis:** Uses Google Text-to-Speech (gTTS) to generate speech in the target language.
- 🎬 **Video Processing:** Uses MoviePy to integrate the generated audio with the original video.
- 🇮🇳 **Indian Regional Language Support:** Helps make digital content accessible to diverse linguistic communities.
- 📥 **Video Upload and Download:** Allows users to upload videos and download the processed output.
- 🖥️ **Web-Based Interface:** Provides a simple interface built using Flask, HTML, and CSS.

## 🗣️ Supported Languages

Global Dub is designed to support multiple Indian languages, including:

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
| Bengali | `bn` |
| Odia | `or` |

*Language availability depends on the language options configured in the application and the support provided by the integrated services.*

## ⚙️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core application development |
| Flask | Web application and backend |
| OpenAI Whisper | Speech recognition and transcription |
| Google Translate (`googletrans`) | Text translation |
| Google Text-to-Speech (`gTTS`) | Speech generation |
| MoviePy | Video and audio processing |
| HTML and CSS | Frontend interface |
| JSON | Structured data and configuration handling |

## 🔄 How It Works

1. **Upload Video:** The user uploads an English-language video through the web interface.
2. **Speech Transcription:** Whisper processes the audio and generates a text transcription.
3. **Language Translation:** The transcribed text is translated into the selected target language.
4. **Dubbed Audio Generation:** gTTS converts the translated text into speech.
5. **Video Processing:** MoviePy integrates the generated audio into the video.
6. **Download Output:** The processed video is made available to the user.

### Workflow

```text
       English Video
             |
             v
    Speech Transcription
      (OpenAI Whisper)
             |
             v
    Text Translation
     (Google Translate)
             |
             v
    Speech Generation
          (gTTS)
             |
             v
    Audio Integration
         (MoviePy)
             |
             v
       Dubbed Video
```

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- Python 3.9 or another compatible Python version
- pip
- Git
- FFmpeg, if required by your MoviePy version

An active internet connection is required for online translation and text-to-speech services. Whisper may also need internet access to download its model if it is not already available locally.

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd Global-Dub
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your repository's actual Git URL.

### 2. Create a Virtual Environment

**Windows PowerShell:**

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks environment activation, use Command Prompt:

```cmd
venv\Scripts\activate.bat
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If a `requirements.txt` file is not present in your repository, install the dependencies listed in your project code and create a requirements file.

### 4. Run the Application

```bash
python main.py
```

Open your browser and navigate to:

```text
http://127.0.0.1:5907
```

If the application uses a different port in your current code, use the configured port instead.

### 5. Generate a Dubbed Video

1. Open the application in your browser.
2. Upload a supported video.
3. Select the target language.
4. Submit the video for processing.
5. Download and review the generated video.

## 📁 Project Structure

```text
Global-Dub/
│
├── main.py
├── requirements.txt
├── package.json
│
├── templates/
│   ├── index.html
│   ├── upload.html
│   └── thankyou.html
│
└── static/
    ├── styles.css
    ├── images and icons
    └── video assets
```

*The structure above is representative. Actual files and directories may vary depending on the version of the project.*

## 🎯 Problem Statement

India has a diverse linguistic landscape, but much of the digital content available online is produced in a limited number of languages. This can make educational resources, informational videos, and other useful content less accessible to people who are more comfortable with regional languages.

Global Dub addresses this challenge by automating key stages of video dubbing, helping users convert English-language video content into selected Indian regional languages through a web-based application.

## 💡 Applications

- 📚 Educational videos in regional languages
- 🎓 Online learning and tutorial localization
- 🎤 Motivational and informational content
- 🌏 Multilingual media accessibility
- 📺 Regional-language video content creation
- 🇮🇳 Improving access to digital content across India

## ⚠️ Limitations

- The current workflow primarily focuses on English-language source videos.
- Translation quality depends on speech transcription and machine translation accuracy.
- Generated speech may differ from the original speaker's voice, tone, and pace.
- The generated audio may not align perfectly with the original video's duration.
- The system does not inherently generate synchronized lip movements.
- Processing time depends on video length, available computing resources, and external service response times.
- Translation and speech generation depend on the availability of the integrated services.

## 🔮 Future Enhancements

- Support for additional source and target languages.
- Automatic source-language detection.
- Improved audio and subtitle synchronization.
- Subtitle generation and downloadable translated transcripts.
- More natural speech generation and improved voice quality.
- Speaker-aware dubbing and better timing alignment.
- Enhanced error handling and temporary file management.
- Secure video uploads and scalable cloud deployment.

## 👩‍💻 Project Objective

Global Dub demonstrates the practical application of artificial intelligence and software development to multilingual media accessibility. By combining speech recognition, machine translation, text-to-speech synthesis, and video processing, the project aims to reduce language barriers and make digital content more accessible to India's diverse linguistic communities.

---

### 🛠️ Built With

**Python · Flask · OpenAI Whisper · Google Translate · gTTS · MoviePy · HTML · CSS**

**Project:** Global Dub — AI-Powered Multilingual Video Dubbing
