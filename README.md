# 🎙️ Telegram Voice AI Chatbot

A voice-enabled AI chatbot for Telegram that combines OpenAI's Whisper for speech recognition, Hugging Face's Zephyr-7B LLM for intelligent responses, and Google Text-to-Speech (gTTS) for voice replies.

This bot allows users to send **voice messages** on Telegram and receive **spoken replies**, creating a seamless voice-to-voice interaction experience.

---

## 🚀 Features

- 🎧 **Voice Input** via Telegram messages
- 🧠 **Intelligent Response Generation** using Zephyr-7B LLM (Hugging Face API)
- 🗣️ **Speech Synthesis** using Google TTS
- 📜 **Local Transcription** using OpenAI’s Whisper (offline)
- 🔁 **Text & Voice Reply** in real-time
- 💡 Supports **text input** as well

---

## 🛠️ Tech Stack

| Component        | Technology Used                         |
|------------------|------------------------------------------|
| Speech Recognition | [Whisper (base)](https://github.com/openai/whisper) |
| LLM Chat Engine  | [Zephyr-7B Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta) |
| Text-to-Speech   | [gTTS (Google Text-to-Speech)](https://pypi.org/project/gTTS/) |
| Messaging Platform | [Telegram Bot API](https://core.telegram.org/bots/api) |
| Audio Handling   | Pydub, FFmpeg                            |
| Programming Language | Python 3.10+                        |

---

## 📦 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/telegram-voice-ai-bot.git
cd telegram-voice-ai-bot
2. Install Dependencies
bash
Copy
Edit
pip install python-telegram-bot requests nest_asyncio python-dotenv gTTS pydub git+https://github.com/openai/whisper.git --quiet
sudo apt-get install ffmpeg -y
🔑 Configuration
Edit the script to add your Telegram Bot Token and Hugging Face Token:

python
Copy
Edit
HF_TOKEN = "your_huggingface_token"
TELEGRAM_TOKEN = "your_telegram_bot_token"
You can optionally use a .env file for better security.

▶️ Usage
Run the bot:
bash
Copy
Edit
python bot.py
Interact with the bot on Telegram:
Send a voice message → Bot replies with voice.

Send a text message → Bot replies with voice.

📈 How It Works
User sends a voice message via Telegram.

Bot downloads and converts audio (OGG → MP3).

Whisper transcribes the voice message into text.

The text is sent to Zephyr-7B via Hugging Face API for a response.

The response is converted to speech using gTTS.

Bot sends the voice response back to the user.

🧪 Example Interaction
User: 🎤 “What is the capital of Italy?”
Bot Response:
📝 “You said: What is the capital of Italy?”
🔊 “The capital of Italy is Rome.”

📚 References
Whisper by OpenAI

Zephyr-7B by Hugging Face

gTTS – Google Text-to-Speech

Telegram Bot API

Pydub

FFmpeg

🔮 Future Enhancements
🌐 Multilingual voice and response support

🧠 Contextual memory with vector databases (e.g., ChromaDB)

🗣️ Use neural TTS (e.g., Bark, ElevenLabs) for realistic voices

💻 Web dashboard (Streamlit) for bot interaction and logs

☁️ Deploy to cloud (Heroku, AWS, Railway)

🤝 Contributing
Contributions are welcome! Please feel free to fork the repo and submit a pull request. Issues and suggestions are also appreciated.

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.

📬 Contact
Author: Asthapuram Chanikya
