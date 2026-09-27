# Voice Assistant

A voice assistant that converts speech to text, generates a response using a language model, and converts the response back to speech.

## Overview

This project builds a simple voice assistant using a combination of speech recognition, a language model, and text-to-speech.

## Pipeline

```text
Voice Input
    ↓
Whisper STT
    ↓
Text
    ↓
Qwen LLM
    ↓
Text Response
    ↓
gTTS
    ↓
Voice Output
```

## Technologies

* Python
* OpenAI Whisper
* Hugging Face Transformers
* Qwen
* gTTS
* Gradio
* PyTorch

## Models

### Speech-to-Text

`openai-whisper`

Whisper is used to convert the user's voice into text.

### Language Model

`Qwen/Qwen2.5-0.5B-Instruct`

Qwen is used to generate a response based on the transcribed text.

### Text-to-Speech

`gTTS`

gTTS converts the generated text response into speech.

## Gradio Interface

The final application uses Gradio and provides:

* Microphone input
* Audio file upload
* Speech transcription
* Assistant text response
* Assistant voice response

## How to Run

1. Install the required libraries.
2. Open the notebook.
3. Run the notebook cells.
4. Launch the Gradio interface.
5. Speak using the microphone or upload an audio file.
6. The assistant returns both text and voice responses.

## Project Structure

```text
voice-assistant-whisper-qwen/
├── voice-assistant.ipynb
└── README.md
```
