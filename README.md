# 🔍 VeracityStream 
> **Byte Quest: PS 03** | Fighting AI Hallucinations with Real-Time Verification

[![Flutter](https://img.shields.io/badge/Frontend-Flutter-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Python](https://img.shields.io/badge/Backend-Python_3.10+-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![Status](https://img.shields.io/badge/Project_Status-Commit_1/8-brightgreen)](#)

---

## 🎯 Vision
Generative AI models often produce factually incorrect information presented with high confidence. **VeracityStream** is an automated verification layer designed to:
* **Decompose AI prose** into individual, testable factual claims.
* **Audit Citations** to identify "ghost" references and broken links.
* **Verify against Truth** by cross-referencing authoritative databases to help users distinguish between reliable and unreliable information.

## 🧠 System Architecture
This diagram outlines the flow from raw AI output to a verified "Veracity Map" in the Flutter app.

```mermaid
graph TD
    subgraph "Client Layer (Flutter)"
        A[Input AI Text/URL] --> B[Interactive Veracity Map]
    end

    subgraph "Intelligence Engine (Python)"
        C{Decomposition Logic}
        D[Claim Extractor]
        E[Link Auditor]
    end

    subgraph "Verification Sources"
        F[Academic DB Search]
        G[Web Status Pinger]
        H[Semantic Scoring]
    end

    A --> C
    C --> D & E
    D --> F --> H
    E --> G --> H
    H --> B

    %% Theming
    style A fill:#f9f9f9,stroke:#333,stroke-width:2px
    style B fill:#02569B,stroke:#02569B,color:#fff,stroke-width:3px
    style H fill:#2ecc71,stroke:#27ae60,color:#fff
