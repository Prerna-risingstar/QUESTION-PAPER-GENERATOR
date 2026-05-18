# 🏛️ AI-Powered College Question Paper Generator

A modern, secure, and beautiful web application built for university faculty to upload course syllabi (.pdf, .docx) and automatically generate structured, academic-standard examination papers matching strict target constraints (marks, format, difficulty, and syllabus coverage).

---

## 🌐 Live URL
Access the live application here:
👉 **[https://question-paper-generator-six.vercel.app/login](https://question-paper-generator-six.vercel.app/login)**

---

## 🚀 Key Features

*   **⚡ Gemini 2.5 Flash Integration**: Rapid generation using OpenRouter API with your custom/default keys.
*   **📂 Syllabus Parsing**: Supports parsing course syllabi from PDF, DOC, and DOCX formats.
*   **🎯 Target Customizer**: Customize exam difficulty (Easy, Medium, Hard) and formats (Mid-Term or End-Semester).
*   **📝 Interactive Workspace Editor**: Full-screen WYSIWYG editor with version control and restoration history.
*   **📥 Multi-Format Exporters**: One-click download of papers compiled into standard **DOCX** or academic **PDF** files.
*   **🔐 Secure Roles**: Role-based access control (Admin, Dean, Faculty) powered by Firebase Authentication.

---

## 🛠️ Quick Local Setup

1. **Clone the repository:**
   ```bash
   cd "c:\projects\QUESTION PAPER GENERATOR"
   ```

2. **Set up virtual environment & install dependencies:**
   ```powershell
   python -m venv venv
   .\venv\Scripts\Activate
   pip install -r requirements.txt
   ```

3. **Provide Firebase Credentials:**
   Place your Firebase private key JSON file in the root folder as `firebase_service_account.json`.

4. **Add Environment Variables:**
   Create a `.env` file in the root directory:
   ```env
   OPENROUTER_API_KEY=your_openrouter_api_key
   FIREBASE_API_KEY=your_firebase_web_api_key
   ```

5. **Start the server:**
   ```bash
   python main.py
   ```
   Open **[http://127.0.0.1:5000](http://127.0.0.1:5000)** in your browser!
