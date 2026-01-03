# 🔍 VeracityStream 
> **Byte Quest: PS 03** | Fighting AI Hallucinations with Real-Time Verification

[![Flutter](https://img.shields.io/badge/Frontend-Flutter-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Python](https://img.shields.io/badge/Backend-Python_3.10+-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![Status](https://img.shields.io/badge/Project_Status-Commit_1/8-brightgreen)](#)

---

## 🚩 The Challenge: AI's "Confidence Gap"
Generative AI models are widely used for research and learning, but they often generate factually incorrect information presented with high confidence. **VeracityStream** addresses the critical risks of:
* **Ghost Citations:** Creation of fake citations and non-existent references that appear legitimate.
* **Broken Trust:** Difficulty for users to distinguish between reliable and unreliable AI-produced info.
* **Misinformation Risks:** Potential for legal, ethical, and professional consequences due to "dead-end" links.

## 🧠 System Architecture
This pipeline illustrates how we transform unstructured AI prose into a verified, color-coded "Veracity Map."

[Image of a sequence diagram for AI hallucination detection system showing user query, LLM response, claim extraction, web/academic search, and final verification]

```mermaid
graph TD
    subgraph Client_Layer ["Client Layer (Flutter)"]
        A[Input AI Text/URL] --> B[Interactive Veracity Map]
    end

    subgraph Intelligence_Engine ["Intelligence Engine (Python)"]
        C{Decomposition Logic}
        D[Claim Extractor]
        E[Link Auditor]
    end

    subgraph Verification_Sources ["Verification Sources"]
        F[Academic DB Search]
        G[Web Status Pinger]
        H[Semantic Scoring]
    end

    A --> C
    C --> D & E
    D --> F --> H
    E --> G --> H
    H --> B

    %% Visibility & Modern Styling
    style Client_Layer fill:#f0f7ff,stroke:#02569B,stroke-width:2px
    style Intelligence_Engine fill:#fffbf0,stroke:#d4a017,stroke-width:2px
    style Verification_Sources fill:#f6fff8,stroke:#2ecc71,stroke-width:2px
    
    style A fill:#ffffff,stroke:#333
    style B fill:#02569B,color:#fff,stroke-width:3px
    style H fill:#2ecc71,color:#fff,stroke-width:2px

## 🎯 Key Objectives & Impact

### ✅ Automated Claim Extraction
Uses NLP techniques to decompose unstructured AI-generated text into individual, testable factual claims.

### 🔗 Citation Audit Engine
- Real-time URL validation  
- Detection of broken, fake, or non-existent citations  
- Metadata verification against academic databases  

### 🎨 Semantic Veracity Mapping
A Flutter-based color-coded UI that visually distinguishes:
- 🟢 Verified claims  
- 🟡 Uncertain or weakly supported claims  
- 🔴 False or unverifiable claims  
