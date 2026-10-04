# StudyMate AI — The Empathetic Technical Study Companion & Exam Coach

> **GitHub Repository**: [https://github.com/guunda/studymate](https://github.com/guunda/studymate)  
> **Submission Project**: An AI-powered study assistant built specifically for a friend who struggles with studying, preparing for exams, or mastering tough technical subjects (Computer Science, Mathematics, Physics, Chemistry, Engineering, and Economics).

---

## 🎯 Problem Statement & Solution

### The Challenge
Students tackling complex technical subjects often face:
1. **Cognitive Overload**: Textbooks present dry, jargon-heavy walls of text with zero intuitive analogies.
2. **Passive Reading Trap**: Rereading notes leads to low retention and exam panic.
3. **Procrastination & Focus Fatigue**: Lack of active recall structure, timer discipline, or ambient focus environments.

### The Solution: StudyMate AI
StudyMate AI transforms scary technical subjects into intuitive, interactive micro-learning experiences:
- **ELI5 Analogy Engine**: Translates complex concepts into real-world metaphors (e.g., explaining Recursion like Russian Matryoshka dolls, or TCP/IP handshakes like phone calls).
- **Feynman Technique Coach**: Prompts the student to explain concepts back in plain English, evaluates retention, detects gaps, and awards XP.
- **Active Recall & 3D Flashcards**: Instant practice quizzes with detailed answer explanations and 3D flip card decks with spaced repetition ratings.
- **Notes Summarizer**: Converts raw lecture notes into 1-page structured revision sheets with mnemonics and export options (PDF Print / Markdown).
- **Mind Map Flowcharts**: Renders step-by-step algorithms, workflows, and system architectures visually using Mermaid.js.
- **Procedural Focus Synthesizer**: Web Audio API ambient audio generator (Rain, Lo-Fi Chords, Brown Noise, 10Hz Alpha Beats) that works **100% offline**.

---

## 🌟 Key Features & Modules

| Module | Description | High-Impact Capability |
| :--- | :--- | :--- |
| 💡 **ELI5 Explainer** | Concept deconstruction into simple analogies | Real-world metaphors, KaTeX LaTeX math rendering, visual mental models, and jargon terms. |
| 🎓 **Feynman Coach** | "Teach the AI back" retention trainer | Natural language evaluation, praise for intuition, gap finder, and gamified XP rewards. |
| 📝 **Quizzes & Decks** | Active recall exam simulator | Multiple-choice practice tests, instant option feedback, 3D flip flashcard decks with spaced repetition. |
| 📚 **Notes Summarizer** | Revision cheat sheet generator | Instant 1-page exam cheat sheets with mnemonics, quick self-tests, and Print PDF / Markdown export. |
| 🧠 **Mind Map Visualizer** | Interactive flowchart renderer | Powered by Mermaid.js with code editor to visually inspect algorithms & systems. |
| ⏱️ **Focus Zone** | Pomodoro timer + Web Audio synth | 25m/5m interval study ring + 100% offline procedural ambient focus sound engine. |
| 📋 **Submission Hub** | Evaluator overview & submission package | 1-click Markdown submission package exporter (`StudyMate_Project_Submission_Report.md`). |

---

## 🛠️ Technology Stack

- **Frontend**: React 19, Vite 8
- **Styling**: Vanilla CSS Design System with CSS Custom Properties, Dark Mode, and Glassmorphism
- **Icons**: Lucide React
- **Math Rendering**: KaTeX (CDN + JS Parser)
- **Diagram Engine**: Mermaid.js
- **Audio Synthesizer**: Web Audio API (procedural oscillator & noise synthesis)
- **Gamification**: Canvas Confetti, LocalStorage persistence
- **AI Integration**: Dual Engine (Smart Built-in Offline Engine + optional Google Gemini / OpenAI live API connectors)

---

## 🚀 Quick Start & Submission Setup

### 1. Installation
```bash
npm install
```

### 2. Run Local Development Server
```bash
npm run dev
```
Open **`http://localhost:5173/`** in your browser.

### 3. Build Production Bundle
```bash
npm run build
```

---

## 📋 Task Submission Verification

- **Submission Package Feature**: Click **"Submission Hub"** in the top navigation bar or banner to view executive summary metrics and export a complete Markdown project report.
- **Offline Reliability**: Works out-of-the-box with zero API key configuration needed, while allowing optional live Gemini or OpenAI keys.
- **Build Verification**: Tested with zero compilation errors (`built in 28.56s`).

---
*Developed with empathy for students striving for technical mastery.*
