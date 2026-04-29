# Athena – Local LLaMA-Based Assistant Chatbot

## Overview

Athena is a locally deployed AI assistant built using a quantized LLaMA-based model. The system demonstrates practical application of large language models in an offline environment with customizable behavior and domain-specific responses.

The project focuses on system integration, prompt engineering, and applied AI usage rather than model training.

---

## Features

* Local LLM deployment (no cloud dependency)
* Custom persona design for domain-specific interaction
* Tunable generation parameters (temperature, top_p, repetition penalty)
* Frontend integration (Flask / Streamlit)
* Real-world testing via sample chat logs

---

## System Architecture

1. Model hosted locally using Oobabooga WebUI
2. Backend powered via llama.cpp
3. Prompt templates define assistant personality and behavior
4. User interaction via CLI / web interface

---

## Project Structure

prompts/
  athena_profile.yaml

logs/
  sample_chat.json

config/
  settings.json

README.md

---

## Prompt Engineering

The assistant behavior is controlled using:

prompts/athena_profile.yaml

Athena is designed to:

* Maintain a polite and academic tone
* Provide structured explanations
* Demonstrate pharmacology awareness

---

## Model Configuration

Example parameters used:

* Model: LLaMA-2 (Echidna Q8)
* Temperature: 0.7
* Top_p: 0.9
* Repetition penalty: 1.1
* Max tokens: 512
* Backend: llama.cpp

Generation parameters were tuned to balance coherence and conversational flexibility.

---

## Sample Outputs

Example interactions are available in:

logs/sample_chat.json

These demonstrate:

* General medical knowledge responses
* Conversational consistency
* Model limitations and safety behavior

---

## Key Learnings

* Practical deployment of local LLM systems
* Prompt engineering for controlled outputs
* Trade-offs between performance and resource usage
* Observed limitations in domain-specific reliability

---

## Disclaimer

This project is for educational purposes only. It does not provide medical advice.

---

## Future Improvements

* Integration with medical datasets (RAG pipeline)
* Improved response validation
* UI enhancements
* Domain-specific fine-tuning
