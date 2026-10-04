*This is a submission for the [Hacktoberfest Weekend Challenge: Build for a Friend](https://dev.to/challenges/hacktoberfest-weekend-2026-10-01)*

## What I Built
I built **StudyMate AI — The Empathetic Technical Companion & Exam Coach** for my friend Alex, who gets overwhelmed whenever studying for complex STEM, computer science, and engineering exams.

### The Problem
When studying technical subjects like Recursion, Derivatives, TCP/IP Networking, Neural Networks, or Organic Chemistry mechanisms, traditional textbooks present dry, jargon-heavy walls of text with zero intuitive analogies. Rereading notes leads to passive reading fatigue, low retention, and exam anxiety.

### The Solution
StudyMate AI transforms scary technical subjects into intuitive, interactive micro-learning experiences:
- **ELI5 Concept Explainer**: Translates complex topics into simple real-world metaphors (e.g., explaining Recursion like Russian Matryoshka dolls or TCP/IP handshakes like phone calls) complete with KaTeX LaTeX formula shortcuts and visual mental models.
- **Feynman Technique Coach ("Teach Me Back")**: Prompts the student to explain concepts back in plain English, evaluates retention with empathetic feedback, spots gaps, and awards XP.
- **Active Recall Quizzes & 3D Flashcards**: Instant practice exams with detailed answer breakdowns and 3D flip card decks with spaced repetition ratings (*Needs Review*, *Good*, *Mastered*).
- **Notes Summarizer & Cheat Sheet Generator**: Converts raw lecture notes into 1-page structured revision sheets with mnemonics and export options (PDF Print & Markdown).
- **Mind Map Visualizer**: Interactive Mermaid.js diagram renderer for flowcharts, system architecture, and algorithms.
- **Procedural Focus Synthesizer**: Web Audio API ambient sound player (Cozy Rain, Lo-Fi Warm Chords, Deep Brown Noise, 10Hz Alpha Binaural Beats) that works **100% offline** with zero external audio assets.

---

## Demo
- **Live Repository**: [https://github.com/guunda/studymate](https://github.com/guunda/studymate)
- **Local Dev Launch**: Run `npm run dev` and open `http://localhost:5173/`

### Interactive Feature Highlights
1. **Empathetic Companion Persona Header**: Real-time level progress, XP tracking, active study streak counter, and audio toggle.
2. **ELI5 Analogy Cards & KaTeX Math**: Glassmorphic interface rendering KaTeX mathematical equations and jargon decoders.
3. **Feynman Coach**: Active recall response evaluator that rewards intuition and provides gentle constructive feedback.
4. **Procedural Web Audio Focus Zone**: Pomodoro interval timer + ambient audio synthesizer created with the Web Audio API.

---

## Code
```javascript
// Web Audio API Procedural Ambient Focus Synthesizer (100% Offline)
class AmbientSynth {
  init() {
    if (!this.audioCtx) {
      const AudioContext = window.AudioContext || window.webkitAudioContext;
      this.audioCtx = new AudioContext();
      this.masterGain = this.audioCtx.createGain();
      this.masterGain.gain.value = 0.5;
      this.masterGain.connect(this.audioCtx.destination);
    }
  }

  generateLoFiChords() {
    // Soft ambient chord progression: Cmaj7 -> Am7 -> Fmaj7 -> G7
    const frequencies = [
      [261.63, 329.63, 392.00, 493.88], // Cmaj7
      [220.00, 261.63, 329.63, 392.00], // Am7
      [174.61, 220.00, 261.63, 329.63], // Fmaj7
      [196.00, 246.94, 293.66, 349.23]  // G7
    ];
    // Generates soothing sine wave chords with lowpass filtering and custom gain envelope
  }
}
```

---

## How I Built It
- **Frontend Framework**: **React 19** + **Vite 8**
- **Design System**: Ultra-premium Glassmorphic CSS design system with CSS Custom Properties, smooth background glow mesh, floating ambient orbs, and Outfit/Inter/Fira Code typography.
- **Math & Diagram Engines**: **KaTeX** for LaTeX mathematical formulas, **Mermaid.js** for visual mental models and flowchart diagrams.
- **Procedural Sound Engine**: Built a Web Audio API procedural synthesizer that generates rain noise, lo-fi chord progressions, brown noise, and 10Hz Alpha binaural beats completely offline.
- **Dual AI Engine**:
  1. **Smart Built-in Offline Engine**: Pre-loaded knowledge base covering major CS, Math, Physics, Chemistry, and Economics topics with ELI5 analogies, formulas, quizzes, and Feynman prompts (works out-of-the-box with zero API keys).
  2. **Live AI API Connectors**: Connects with Google Gemini API (`gemini-1.5-flash`) and OpenAI API (`gpt-4o-mini`) for real-time dynamic study breakdowns when an API key is provided.
- **AI Pair Programming**: Built with assistance from **Google Antigravity AI Agent** for prompt design, code linting (`oxlint`), and production build verification.

---

## Why Does Open Innovation Matter?
Open innovation and client-side web technologies make empathetic education accessible to every student everywhere, regardless of financial resources or internet reliability.

1. **Zero Paywalls & Universal Access**: By relying on open web standards (Web Audio API, KaTeX, Mermaid.js) and an offline-first knowledge engine, students can study anytime without needing expensive API subscriptions or high-speed data.
2. **Complete Data Privacy**: A student's personal study notes, Feynman explanations, and learning struggles stay 100% local in their browser via LocalStorage, ensuring total privacy.
3. **Extensibility & Customization**: Open architecture allows educators and developers to fork the codebase, add custom subject decks, or integrate local open-weight LLMs (e.g., Ollama / LM Studio).

---

## My Agent Session
Developed and refined with pair-programming assistance from **Google Antigravity AI Agent** during the build session for automated code auditing, lint cleaning (`oxlint`), and production build verification (`vite build`).

---

## Prize Categories
- **Hacktoberfest Weekend Challenge: Build for a Friend**
- **Open Innovation & Web AI Category**
