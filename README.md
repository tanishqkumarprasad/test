# 🔍 VeracityStream  
> **Byte Quest: PS 03** | *Fighting AI Hallucinations with Real-Time Verification*

[![Flutter](https://img.shields.io/badge/Frontend-Flutter-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Python](https://img.shields.io/badge/Backend-Python_3.10+-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![Status](https://img.shields.io/badge/Project_Status-Commit_1/8-brightgreen)](#)

---

## 🚩 The Challenge: AI’s “Confidence Gap”

Generative AI models are widely used for research, learning, and decision-making.  
However, they often generate **factually incorrect information with high confidence**, leading to trust, legal, and ethical risks.

**VeracityStream** is an automated verification layer designed to address:

- **Fabricated Facts** – Claims without empirical evidence  
- **Ghost Citations** – Fake, broken, or non-existent references  
- **Misinformation Risks** – Harm caused by unreliable AI-generated content  

---

## 🧠 System Overview
## 🧠 System Overview

<p align="center">
  <img src="assets/veracitystream-architecture.png"
       alt="VeracityStream System Architecture"
       width="700">
</p>

**Flow:**

1. User inputs AI-generated text or a URL  
2. Text is decomposed into individual factual claims  
3. Claims and citations are verified using academic and web sources  
4. Results are scored and visualized in a color-coded UI  

---

## 🎯 Key Objectives & Impact

### ✅ Automated Claim Extraction
Breaks unstructured AI text into independent, testable factual units using NLP.

### 🔗 Citation Audit Engine
- Validates URLs in real time  
- Detects fake or broken references  
- Verifies metadata against academic databases  

### 🎨 Semantic Veracity Mapping
A Flutter-based UI that highlights:
- 🟢 Verified claims  
- 🟡 Uncertain claims  
- 🔴 False or unverifiable claims  

---

## 🛠️ Tech Stack

### Frontend
- Flutter (Mobile & Web)

### Backend
- Python 3.10+
- FastAPI
- LangGraph

### Verification APIs
- OpenAlex (Academic search)
- Crossref (Citation metadata)
- SerpAPI (Web verification)

---

## 📊 Success Metrics

- **Detection Accuracy:**  
  > 90% identification of fabricated citations and invalid references

- **Verification Latency:**  
  Under 3 seconds per factual claim

- **Source Reliability:**  
  Preference for peer-reviewed and authoritative sources

---

## 🚀 Build Milestones

- [x] Commit 1: Initial Vision & Strategic Roadmap  
- [ ] Commit 2: Flutter Project Scaffolding & Theme  
- [ ] Commit 3: Backend – NLP Claim Extraction  
- [ ] Commit 4: Citation Metadata Validator  
- [ ] Commit 5: Real-Time Verification & Scoring API  
- [ ] Commit 6: Flutter ↔ Backend API Integration  
- [ ] Commit 7: Flutter Veracity Highlight UI  
- [ ] Commit 8: Final Polish & Documentation  

---

## 📌 Vision

> *“Trust is the missing layer in AI outputs. VeracityStream makes truth visible.”*
