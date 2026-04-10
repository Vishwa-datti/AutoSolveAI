# 🚀 AutoSolveAI

## 💡 Overview

AutoSolveAI is a multi-agent AI system that processes PDFs containing questions, generates answers, validates correctness, and provides feedback in real time.

This project was built to solve the problem of students getting **incorrect or inconsistent answers** from different sources, by improving answer accuracy and reliability.
## 📊 Architecture Diagram

Postman → Webhook → PDF Extraction → Solver Agent → Validator Agent → Telegram


---

## ⚙️ System Workflow

1. A PDF (containing only questions) is sent via Postman
2. The request is received through a webhook in Make.com
3. Text is extracted from the PDF
4. The questions are sent to the **Solver Agent**
5. Answers are generated
6. The answers are passed to the **Validator Agent**
7. Final output is sent to Telegram

---

## 🧠 Multi-Agent Architecture

### 🧠 Solver Agent

* Takes extracted questions
* Generates answers using AI

### 🔍 Validator Agent

* Evaluates correctness of answers

#### ✅ Correct

* Sends final answer directly to Telegram

#### ❌ Incorrect

* Identifies the mistake
* Provides the correct answer
* Gives a clear explanation

#### ⚠️ Partially Correct

* Highlights correct parts
* Points out incorrect parts
* Provides explanation

---

## 🎯 Key Features

* Multi-agent system design
* Automated PDF question processing
* Answer validation mechanism
* Real-time feedback through Telegram
* Focus on improving learning accuracy

---

## 🛠️ Tech Stack

* Make.com (Automation)
* Postman (API testing)
* Telegram (Output delivery)

---

## 📊 Architecture Flow

Postman → Webhook → PDF Extraction → Solver Agent → Validator Agent → Telegram

---

## 📦 Project Files

* `blueprint.json` → Make.com workflow

---

## 🎓 Use Case

This system is useful for students (especially in ECE) who:

* struggle to find correct solutions
* want to verify answers
* need clear explanations for mistakes

---

## 🚀 Future Improvements

* Support for handwritten PDFs
* Add confidence scoring
* Improve domain-specific accuracy
* Integration with learning platforms

---

## 🧠 Concept

This project shows how multi-agent systems can improve AI reliability by separating:

* Answer Generation
* Answer Validation

