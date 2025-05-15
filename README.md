# Fine-Tuning LLaMA3 with LoRA and QLoRA for the STT System

This repository contains the code and experiments developed for the undergraduate thesis of Bruna Dias Pupo. The project involved fine-tuning LLaMA3 models for telemedicine applications, resulting in a specialized technical chatbot designed to assist internal users of the STT (Santa Catarina Telemedicine and Telehealth System), specifically in the dermatology module.

## 📚 Context

As the STT system grows in complexity and volume of data, it becomes increasingly challenging for medical professionals to quickly access relevant technical information. This project explores the feasibility of applying large language models (LLMs) fine-tuned with domain-specific data to support information retrieval and technical assistance in this scenario.

## 🧠 Model Overview

- **Base model**: Meta LLaMA 3 - 7B
- **Fine-tuning techniques**: `LoRA` and `QLoRA` for memory optimization
- **Final format**: Converted to GGUF for local inference
- **Execution environment**: `Ollama` + `Open WebUI`
- **Dataset**: Built from STT-Dermatology technical manuals and documentation

## ⚙️ Tools & Technologies

- Python + Jupyter Notebook
- Hugging Face `transformers`, `peft`, `datasets`
- `bitsandbytes`, `accelerate`
- Ollama (model serving)
- Hugging Face Hub (model sharing)
- Open WebUI (graphical user interface)
- GPU A100 (Google Colab environment)

## 🧪 Results

The fine-tuned model was evaluated by STT’s internal technical team:

- Average score of **4.11 / 5.0** in technical support performance
- Positive feedback on usability
- Identified areas for improvement: answer consistency and hallucination reduction

## 🗂 Project Structure

```
├── FineTuning_STT_Llama3.ipynb    # Notebook with the fine-tuning pipeline
├── dataset/                       # Input data for training
├── exported-model/                # Model files in GGUF format
└── interface/                     # Scripts for Ollama + WebUI integration
```

## 🚀 How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open and run `FineTuning_STT_Llama3.ipynb` (preferably on Google Colab with GPU)

3. Start the local model server:
   ```bash
   ollama serve
   ```

4. Use Open WebUI to chat with your fine-tuned model.

## 📄 Reference

This project was developed as part of the undergraduate thesis:

> **Using Large Language Models to Support Telemedicine Systems**  
> Bruna Dias Pupo — Federal University of Santa Catarina (UFSC)  
> Department of Information Science — 2024

## 👩‍💻 Author

Bruna Dias Pupo  
[GitHub](https://github.com/brunapupo) • [LinkedIn](https://linkedin.com/in/brunapupo)  
FullStack Developer | AI Research in Healthcare
