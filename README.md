# 🎙️ AI-Audio-to-Meeting-Minutes-Generator

An end-to-end AI application that converts meeting audio into **structured meeting minutes** using open-source models. Recommended to use T4 GPU on Colab 
## Note: To view the code please download the .ipynb file as it may not render properly in Github because of certain technical issues from Github for .ipynb files

---

## 🚀 Features

- 🎧 Audio → Text using **Whisper (ASR)**
- 🧠 Text → Structured Minutes using **Llama 3 (LLM)**
- 📄 Automatic **PDF generation**
- 🌐 Interactive UI using **Gradio**
- ⚡ Memory-efficient inference using **4-bit quantization (BitsAndBytes)**

---

## 🧠 How It Works
- Audio Input → Whisper → Transcription → LLM (LLAMA) → Structured Minutes → PDF Generator → Downloadable File
  

---

## 🛠️ Tech Stack

- **Transformers (Hugging Face)** – model loading & pipelines  
- **Whisper** – speech-to-text  
- **Llama 3 (Instruct)** – text generation  
- **BitsAndBytes** – 4-bit quantization  
- **Gradio** – web UI  
- **FPDF** – PDF creation  
- **PyTorch** – backend framework  

---


# 🧩 Core Components
## 1. Speech Recognition (Whisper)

Converts audio input into text transcription.

## 2. LLM (Llama 3)

Takes transcription and generates:

- Summary
- Key Points
- Action Items

## 3. Quantization (BitsAndBytes)

Reduces model size using 4-bit precision:

- Lower memory usage
- Faster inference
- Minimal accuracy loss

## 4. Gradio UI

Provides:

- Audio upload / recording
- Live progress tracking
- Output display
- PDF download

## ⚙️ Installation

```bash
pip install transformers accelerate bitsandbytes
pip install gradio fpdf
```
