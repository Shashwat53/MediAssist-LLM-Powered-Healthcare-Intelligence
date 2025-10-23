# MediAssist-LLM-Powered-Healthcare-Intelligence
Built two RAG-based systems : Patient Engagement Assistant and Medicaid Policy Navigator — using open-source LLMs (Qwen-2.5, BGE, MarianMT) to simplify medical guidance and make Medicaid policies searchable. Fully modular, bilingual, and Colab-deployable for transparent, real-time healthcare retrieval.
# 🏥 MediAssist – LLM-Powered Healthcare Intelligence

**Overview**  
MediAssist is a dual-system, Retrieval-Augmented Generation (RAG)–based framework designed for healthcare knowledge retrieval and Medicaid policy navigation. It leverages open-source Large Language Models (LLMs) such as **Qwen-2.5**, **BGE**, and **MarianMT** to simplify medical guidance, make Medicaid policies searchable, and enable transparent, multilingual healthcare intelligence.

## 🚀 Features
- **Two RAG-based systems:**
  - 🩺 **Patient Engagement Assistant** – Answers medical and healthcare-related questions through contextual retrieval and generative reasoning.  
  - 🏛️ **Medicaid Policy Navigator** – Parses and summarizes state and federal Medicaid policy documents for improved accessibility.

- **Open-Source LLM Stack**
  - Qwen-2.5 for generation and reasoning  
  - BGE for dense + sparse hybrid retrieval  
  - MarianMT for multilingual translation and cross-lingual support

- **Core Capabilities**
  - Fully modular architecture (document ingestion → embedding → retrieval → generation)  
  - Colab-deployable design for quick experimentation  
  - Bilingual and policy-compliant retrieval  
  - Integrated monitoring and explainability layer for transparency

## 🧠 System Architecture
```mermaid
flowchart LR
  A[Input Query] --> B[Document Retriever (FAISS + BGE)]
  B --> C[Context Generator]
  C --> D[LLM (Qwen-2.5)]
  D --> E[Response Generator]
  E --> F[Answer + Source Citations]
