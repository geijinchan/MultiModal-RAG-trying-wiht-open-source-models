# Multimodal Retrieval and Generation System

This project demonstrates a multimodal retrieval-augmented generation system that processes videos to extract images, audio, and transcribe text, followed by embedding and indexing with CLIP, retrieval with FAISS, and summarization and augmentation using advanced models like LLaVA and LLaMA.

## Features

- **Video Processing**: Converts a video into frames (images) and extracts the audio.
- **Audio Transcription**: Uses OpenAI's Whisper model for transcribing audio to text.
- **Image and Text Embedding**: Utilizes the CLIP model to create embeddings for images and text.
- **Multimodal Retrieval**: Combines image and text embeddings, indexes them using FAISS, and retrieves relevant data based on a text query.
- **Augmentation**: LLaVA model provides image descriptions and enhances retrieval results.
- **Summarization**: LLaMA 3.1 is used to summarize retrieved text.
  
## Project Workflow

1. **Download Video**: Fetch video from YouTube.
2. **Extract Frames**: Converts the video into a series of images.
3. **Extract Audio and Transcribe**: Extracts audio and uses Whisper for transcription.
4. **Create Embeddings**: Generates embeddings for both images and text using the CLIP model.
5. **Indexing and Retrieval**: Uses FAISS to index and retrieve relevant image and text data based on queries.
6. **Augmentation**: Combines retrieved images and text and enhances the description with LLaVA.
7. **Summarization**: Summarizes the combined data using LLaMA.

## Models Used

- **Whisper**: For speech-to-text conversion.
- **CLIP**: For embedding images and text.
- **FAISS**: For efficient retrieval using indexed embeddings.
- **LLaVA**: For augmenting image descriptions.
- **LLaMA 3.1**: For summarizing the results.

## Installation

```bash
pip install annoy sentence-transformers moviepy pytube pytubefix pydub openai-whisper SpeechRecognition faiss-cpu groq



