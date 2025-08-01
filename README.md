# 🎤 TalkBot

This project is a voice-based chatbot interface powered by OpenAI's GPT-4, using Gradio for the UI and SpeechRecognition for converting audio input to text. Users can speak into their microphone, and the chatbot will respond intelligently using conversational memory.

## 📦 Features

🎙️ Voice input through the microphone
🤖 Conversational AI using GPT-4 via LangChain
🧠 Memory buffer to retain context between interactions
🌐 Web interface using Gradio (can be shared via a link)


## 🛠️ Requirements

Install the required packages using pip:

pip install gradio openai langchain python-dotenv SpeechRecognition

Also ensure you have ffmpeg installed on your system, which is required for audio processing by Gradio.

## 🔐 Setup

Create a .env file in the same directory with your OpenAI API key:

OPENAI_API_KEY=your_openai_api_key_here

## 🚀 How to Run

Launch the chatbot by running the Jupyter notebook or executing the Python code:

jupyter notebook gpt4_voicechat.ipynb

The interface will open in your browser. Speak into your microphone, and the chatbot will respond.


## 🧩 How It Works

Gradio captures audio input.
SpeechRecognition converts audio to text.
LangChain feeds the recognized text to GPT-4 with memory support.
The chatbot responds, and the response is displayed in the interface.


📌 Notes

If the chatbot cannot understand the audio, it will return a polite error message.
The conversation memory allows GPT-4 to understand context across turns.




