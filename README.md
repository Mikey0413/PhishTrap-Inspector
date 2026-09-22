# 🛡️ PhishTrap // Autonomous Offer & Phishing Inspector

An edge-ready, client-side cybersecurity inspection engine engineered to analyze employment offer letters, candidate portals, and onboarding communications. It parses unstructured text, images (OCR), and PDF contracts to detect advance-fee equipment scams, deposit traps, and domain spoofing with zero false positives on authentic employment contracts.

---

## ⚡ Problem Statement
Job seekers, interns, and renters lose millions of dollars each year to advance-fee check laundering schemes, pay-for-equipment fraud, and refundable security deposit traps that bypass standard email spam filters. 

**The Challenge:** Build an autonomous single-page security scanner that ingests offer documents, extracts indicators of compromise (IOCs), validates domain and payment vectors, and calculates an explainable **Dynamic Scam Threat Index (0–100%)**.

---

## 🔬 Core Capabilities & Architecture

- **Multi-Modal Intake Engine:**
  - **Images & Screenshots:** Client-side Optical Character Recognition (OCR) powered by `Tesseract.js` to parse captured offer screenshots and cheques.
  - **PDF Contracts:** Digital text extraction powered by Mozilla's `PDF.js` without uploading sensitive candidate files to external third-party servers.
  - **Directory & Multi-File Batching:** Direct support for raw `.txt`, `.eml`, screenshots, and folder batch uploads (`webkitdirectory`).
- **Context-Aware Bidirectional Heuristic Engine:**
  - **Extortion Vector Scoring:** Flags advance-fee equipment check schemes, untraceable P2P transfers (Crypto, Zelle, Cash App, Gift Cards), upfront background check deposits, and anonymous chat routing (Telegram / WhatsApp).
  - **Legitimacy Dampeners (False-Positive Suppression):** Awards integrity credits when authentic statutory terms (CTC, PF, Gratuity, ESIC, Non-Disclosure, Probation Clauses, company-funded asset provisioning) are present, ensuring legitimate offer letters are scored accurately as **SAFE (0/100%)**.
- **Per-Input Forensic Breakdown:**
  - Evaluates each uploaded file, document, or pasted email body independently with its own threat gauge (`XX/100%`) and itemized finding count.
- **Incident Audit Dossier Export:**
  - One-click markdown clipboard export and print-to-PDF formatting for reporting incidents to SOC teams or cybercrime portals.

---

## 🛠️ Tech Stack

- **Frontend & UI:** Single-Page Architecture, HTML5, Tailwind CSS (Clean Light & Dark Mode)
- **Document & Image Parsing:** Mozilla `PDF.js`, `Tesseract.js` (OCR)
- **Heuristic Engine:** Client-Side Pattern Matching & Dynamic Scoring Algorithm
- **Deployment:** Vercel / GitHub Pages (Zero-config, static execution)

---

## 🚀 Quick Start & Local Setup

### 1. Clone the Repository
```bash
git clone [https://github.com/](https://github.com/)<your-username>/phish-inspector.git
cd phish-inspector
