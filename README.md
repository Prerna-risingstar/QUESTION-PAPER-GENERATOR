# 🏛️ AI-Powered College Question Paper Generator

An advanced, secure, and beautiful web application built for university faculty networks. This system allows standard personnel to upload course syllabi (.pdf, .docx) and automatically generate structured, academic-standard examination papers matching strict target constraints (marks, format, difficulty, and syllabus coverage). 

The platform leverages **Google Gemini 2.5 Flash** (via BYOK OpenRouter routing) to generate papers in seconds, ensuring **zero rate limits** and **completely free operations**.

---

## 🎨 Premium Visual Interface

The web application has been tailored to a stunning, modern **Indigo, White, and Light Pink theme** with full dark-canvas contrast:
- **Global Background**: A rich, deep luxurious Indigo (`#1E1B4B`).
- **Floating Surfaces**: High-contrast, clean White cards (`#FFFFFF`) with sleek dark indigo text.
- **Accents**: Soft vibrant Pink highlights (`#FF80B5`) for active alerts, secondary details, and drag-and-drop file containers.
- **Academic Writing Room**: A dedicated dark-mode document workspace with revision logs and automated AI compliance cross-referencing.

---

## 🚀 Key Features

*   **⚡ Google Gemini 2.5 Flash (BYOK)**: Integrated directly with personal Google AI Studio keys via OpenRouter to bypass public free-tier rate limits (429 errors) and avoid credit requirements (402 errors).
*   **📂 Multi-Format Syllabus Parser**: Seamless extraction of PDF, DOC, and DOCX syllabus outlines.
*   **🎯 Adaptive Question Paper Customizer**:
    *   *Exam Formats*: Mid-Term (50 Marks / 2 Hours) or End-Semester (100 Marks / 3 Hours).
    *   *Difficulties*: Easy (Recall & Basic), Medium (Balanced), or Hard (Application & Analysis).
    *   *Uniqueness Enforcement*: The system cross-references previous outputs for the subject to ensure newly generated papers contain unique questions!
*   **📝 Interactive Workspace Editor**: Full-screen WYSIWYG workspace designed like Microsoft Word. Features manual saves and instant revision-history snapshots.
*   **📑 Immutable System Audit Logs**: A secure ledger tracking all generations and edits by faculty members.
*   **🔐 Firebase Authentication**: Enterprise-grade role-based clearance (Standard Faculty vs. Systems Administrator) with standard personnel management.
*   **📥 Native Document Exporter**: One-click download of generated papers in beautifully compiled **DOCX** and academic-styled **PDF**.

---

## 🛠️ Tech Stack

*   **Backend**: Flask (Python 3)
*   **Database**: SQLite (SQLAlchemy / raw sqlite3 for revision history and system logs)
*   **Authentication**: Firebase Admin SDK (Identity & Custom Role Claims)
*   **AI Engine**: OpenRouter API (`google/gemini-2.5-flash`)
*   **Export Drivers**: `python-docx` & `fpdf2`

---

## ⚙️ Installation & Setup

Follow these steps to boot the local environment on Windows:

### 1. Clone & Position
Ensure your directory structure is positioned within your local workspace:
```bash
cd "c:\projects\QUESTION PAPER GENERATOR"
```

### 2. Set Up Virtual Environment
Create and activate a isolated python workspace:
```powershell
python -m venv venv
.\venv\Scripts\Activate
```

### 3. Install Dependencies
Install all library packages listed in the requirements file:
```bash
pip install -r requirements.txt
```

### 4. Bind Firebase Credentials
1. Retrieve your Firebase Service Account private key JSON from your Firebase Console (**Project Settings -> Service Accounts -> Generate New Private Key**).
2. Save the downloaded JSON file directly in the root directory and rename it to:
   `firebase_service_account.json` *(Note: This file is automatically ignored by Git to protect your private keys).*

### 5. Start the Server
Boot the local development server:
```bash
python main.py
```
Open your browser and navigate to: **[http://127.0.0.1:5000](http://127.0.0.1:5000)**

---

## 🔑 AI Key Setup (BYOK - Bring Your Own Key)

To ensure completely free, rate-limit-free generations:
1. Log into your **OpenRouter** account.
2. Go to **Integrations** -> **Google AI Studio** and paste your free Google Gemini API Key.
3. In the application, navigate to **Settings** and save your secure OpenRouter API Key.
4. The system will automatically leverage your linked Google API key to route requests securely and completely for free!

---

## 📄 License
This repository is configured for academic and institution deployment under the terms of the Global University of Technology network. Unauthorized sharing of credentials or system logs is strictly prohibited.
