<div align="center">

# 🛡️ PhishGuard
### AI-Powered Multi-Modal Phishing Detection System

**Detect • Explain • Protect**

An intelligent phishing detection platform that combines **Machine Learning**, **Natural Language Processing**, and **Vision-Language Models** to identify phishing attacks across URLs, Emails, QR Codes, and Website Screenshots.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi)
![XGBoost](https://img.shields.io/badge/XGBoost-URL%20Detection-orange?style=for-the-badge)
![RoBERTa](https://img.shields.io/badge/RoBERTa-NLP-red?style=for-the-badge)
![LLaVA](https://img.shields.io/badge/LLaVA-Vision--Language-purple?style=for-the-badge)


</div>

---

# 📖 Overview

Phishing remains one of the most common and dangerous cyber threats. Most existing phishing detectors rely on **only one source of information**, such as URLs or email content, making them ineffective against increasingly sophisticated attacks.

**PhishGuard** addresses this limitation by introducing a **Multi-Modal AI-based phishing detection system** that simultaneously analyzes:

- 🌐 URLs
- 📧 Email Content
- 🖼️ Website Screenshots
- 📱 QR Codes

Unlike conventional systems, PhishGuard not only detects phishing attempts but also **explains why a resource is malicious**, enabling users to make informed security decisions.

---

# ✨ Key Features

## URL Phishing Detection

- Detects malicious URLs using **XGBoost**
- URL feature engineering
- Domain intelligence
- WHOIS lookup
- URL risk scoring
- High-speed inference

---

## Email Phishing Detection

- Transformer-based phishing email classifier
- Fine-tuned **RoBERTa**
- Context-aware text understanding
- Supports long-form emails

---

## Screenshot Analysis

- Website screenshot inspection
- Visual phishing detection
- Brand impersonation identification
- Interface similarity analysis

---

## Explainable AI

Traditional phishing detectors simply return:

> "This website is malicious."

PhishGuard goes one step further.

Using **LLaVA**, it generates natural language explanations describing:

- suspicious visual elements
- fake login pages
- deceptive content
- security risks

making predictions understandable for end users.

---

## Safe URL Preview

Users can safely preview webpages without opening potentially harmful websites.

This minimizes accidental interaction with malicious content.

---

## QR Code Detection

Many phishing attacks now use QR codes.

PhishGuard

- extracts URLs
- analyzes embedded links
- performs complete phishing assessment

without requiring manual inspection.

---

# System Architecture

```
                    User Input
                         │
      ┌──────────────────┼──────────────────┐
      │                  │                  │
     URL             Email Text        QR Code
      │                  │                  │
      ▼                  ▼                  ▼
  XGBoost           RoBERTa          QR Decoder
      │                  │
      └───────────┬──────┘
                  │
                  ▼
         Screenshot Capture
                  │
                  ▼
               LLaVA
                  │
                  ▼
       Explainable AI Engine
                  │
                  ▼
        Threat Assessment Report
                  │
                  ▼
          FastAPI Web Dashboard
```

---

# Technology Stack

| Category | Technologies |
|-----------|--------------|
| Backend | FastAPI |
| Programming Language | Python |
| Machine Learning | XGBoost |
| NLP | RoBERTa |
| Vision-Language Model | LLaVA |
| Deep Learning | PyTorch |
| Frontend | HTML, CSS, JavaScript |
| APIs | WHOIS |

---

# Project Structure

```
---

# 📊 Datasets

### URL Dataset

- Malicious URLs
- Benign URLs

Used for training the XGBoost classifier using handcrafted URL features.

---

### Email Dataset

Collection of legitimate and phishing emails used to fine-tune the RoBERTa model.

---

# 📈 Model Performance

| Module | Model | Accuracy |
|---------|--------|-----------|
| URL Detection | XGBoost | **99.70%** |
| Email Detection | RoBERTa | **98.95%** |

---

# ⚙️ Detection Pipeline

```
User Input
      │
      ▼
Input Classification
      │
      ▼
Relevant AI Model
      │
      ▼
Threat Prediction
      │
      ▼
Explainable AI
      │
      ▼
Final Threat Report
```

---

# 🚀 Getting Started

## Clone the Repository

```bash
git clone https://github.com/your-username/phishguard.git

cd phishguard
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Start the Server

```bash
uvicorn main:app --reload
```

---

Open

```
http://127.0.0.1:8000
```

---

# 💡 Application Modules

✔ URL Detection

✔ Email Detection

✔ Screenshot Analysis

✔ QR Code Analysis

✔ Safe URL Preview

✔ Domain Intelligence

✔ WHOIS Analysis

✔ Explainable AI

✔ Interactive Dashboard

---

# 🎯 Future Work

- Browser Extension
- Chrome & Edge Integration
- Gmail Plugin
- Mobile Application
- Live Threat Intelligence
- Multi-language Email Detection
- Cloud Deployment
- Redirect Chain Analysis
- Enhanced Visual Reasoning
- Real-time Website Monitoring

---

# 📚 References

- XGBoost for Phishing URL Detection
- RoBERTa for Email Classification
- LLaVA Vision-Language Model
- Kaggle Phishing Datasets

---

# 🌟 Why PhishGuard?

Unlike traditional phishing detection tools that analyze only a single input, **PhishGuard** combines **URL intelligence**, **email understanding**, **visual reasoning**, and **explainable AI** into one unified platform.

This multimodal approach improves detection accuracy while helping users understand *why* a website or email is potentially malicious, making cybersecurity more transparent, trustworthy, and effective.

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a Star!

by the **PhishGuard Team**

</div>
