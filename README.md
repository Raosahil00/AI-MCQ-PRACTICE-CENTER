# AI-MCQ-PRACTICE-CENTER


# 👑 AI MCQ Practice Center – **Royal Edition**

A **premium, elegant, and intelligent** web application for creating, practicing, and analyzing multiple-choice question quizzes.
This tool leverages **Google Gemini API** to generate questions from text, topics, or PDFs, and provides **detailed performance analytics** to help learners achieve their goals in style.

---

## ✨ Key Features

### 🤖 AI-Powered Question Generation

* Go beyond manual entry — just **provide a topic, block of text, or stylistic instructions**, and let AI generate a **custom quiz** for you.

### 📄 Intelligent PDF Processing

* Upload any **text-based PDF**, specify a page range, and instantly extract its content for AI question generation.

### 🏷 AI Question Categorization

* Automatically sorts generated questions into **Math, English, Reasoning, or General Knowledge** categories.

### 🖱 Interactive Quiz Experience

* **Horizontal Navigator** – Sleek scrollable bar to view progress & jump to any question.
* **Category Filtering** – Focus on specific subjects mid-quiz.
* **Live Progress Tracking** – Real-time status:

  * ✅ Answered (Green)
  * ⏩ Skipped (Red)
  * ⭐ Current (Gold)

### 📊 Comprehensive Performance Analysis

* **Detailed Dashboard** – Get instant feedback on score, accuracy, average speed, and total time.
* **Goal Tracking** – Set a target score & visually compare results.
* **Spider Chart Breakdown** – See strengths & weaknesses beautifully.
* **Review & Re-attempt** – Reattempt only skipped or incorrect questions.
* **Save & Resume** – Resume incomplete sessions anytime — progress is saved in-browser.

### 👑 Elegant & Premium Design

A luxurious **royal-themed UI**, with elegant typography, calming colors, and a **minimal, expensive feel** — making learning enjoyable and aesthetic.

---

## 🔄 Workflow

1. **Set Your Goal** – Define your target score & optional time limit.
2. **Add Questions:**

   * **AI Generation** – Provide topic/context & let AI create the questions.
   * **Upload PDF** – Extract content from selected pages & use it as context.
   * **Manual Entry** – Add your own questions/answers individually.
3. **Take the Quiz** – Use filters, jump with the navigator, and track real-time progress.
4. **Review Results** – Analyze performance, review mistakes, and reattempt missed questions.

---

## ⚠️ Handling PDFs with Images (OCR)

This app **only works with text-based PDFs** — it cannot read scanned PDFs.

**Solution:**
Use Google Drive’s free **OCR feature**:

1. Upload the PDF to Google Drive.
2. Right-click → **Open with → Google Docs**.
3. Copy the extracted text and paste it into the app’s “Context / Paragraph” field.

---

## 🚀 Local Setup

To run AI-powered features locally, you must add your own **Google Gemini API Key**.

**Steps:**

1. Get your free API key from **[Google AI Studio](https://aistudio.google.com/)**.
2. Open `index.html` and find the `generateQuestionsFromText` function (\~line 470).
3. Paste your key in place of the placeholder:

```javascript
// Inside the generateQuestionsFromText function...
try {
    const apiKey = "YOUR_API_KEY_HERE"; // <--- PASTE YOUR KEY HERE
    if (!apiKey || apiKey === "YOUR_API_KEY_HERE")
        throw new Error("API key is missing.");
    // ... rest of the function
```

