# 🎓 LearnLab
**Personalized Learning Platform with Adaptive Curriculum**

> **An intelligent learning platform that diagnoses knowledge gaps, generates personalized lessons, and adapts curriculum in real-time based on performance—powered by LangGraph and AI.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![LangGraph](https://img.shields.io/badge/LangGraph-AI_Agents-purple.svg)](https://langchain-ai.github.io/langgraph/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ What It Does

LearnLab is an adaptive learning platform that uses a **LangGraph-powered state machine** to create truly personalized educational experiences:

1. **Assess Knowledge Gaps** — Diagnostic quizzes identify weak skills using mastery modeling
2. **Generate Adaptive Lessons** — RAG-powered content generation creates targeted lessons with exercises
3. **Evaluate Performance** — Automated quiz generation and intelligent grading with detailed feedback
4. **Adapt Curriculum** — Real-time mastery updates and intelligent recommendations for next steps

All orchestrated seamlessly through a polished, learner-centric interface.

---

## 🎯 Core Features

### 🤖 **AI-Powered Learning Engine**
- **LangGraph Orchestration** — Multi-node state machine managing the complete learning loop
- **RAG Content Generation** — Vector search retrieves relevant content, then generates pedagogically sound lessons
- **Intelligent Recommendations** — Mastery-based skill gap analysis drives personalized next steps
- **Structured AI Outputs** — JSON schemas ensure consistent, high-quality generated content

### 📊 **Adaptive Curriculum System**
- **Mastery Tracking** — Per-skill proficiency scores (0.0–1.0) updated after each assessment
- **Gap Analysis** — Automatic identification of knowledge gaps with prioritized recommendations
- **Dynamic Lesson Generation** — Lessons tailored to specific skill gaps, not generic content
- **Progressive Difficulty** — Exercises and quizzes adapt to learner's current level

### 🎨 **Polished Learning UX**
- **Dashboard Overview** — Mastery visualization, streak tracking, and achievement system
- **Interactive Lessons** — Rich markdown content with embedded exercises and explanations
- **Quiz Runner** — Voice input support, real-time feedback, and detailed per-question analysis
- **Analytics Dashboard** — Comprehensive progress tracking with skill breakdown and activity logs

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🎯 **Diagnostic Assessment** | Initial knowledge gap detection |
| 📚 **Adaptive Lessons** | RAG-generated content with sections and exercises |
| 📝 **Smart Quizzes** | Auto-generated assessments with MCQ and short-answer questions |
| 📈 **Mastery Model** | Per-skill proficiency tracking with automatic updates |
| 🎓 **Recommendations** | Intelligent next-step suggestions based on gaps |
| 💬 **AI Chat Assistant** | Context-aware learning support during lessons |
| 📊 **Analytics Dashboard** | Detailed progress visualization and skill breakdown |
| 🏆 **Achievements & Streaks** | Gamification elements to maintain engagement |
| 🔔 **Study Reminders** | Browser notifications for learning consistency |
| 📥 **Progress Export** | Download learning data in JSON or text format |
| 🎤 **Voice Input** | Speech-to-text for quiz answers |
| 💻 **Code Playground** | Interactive coding exercises with live execution |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16.0.10** | React 19.2 with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling |
| **shadcn/ui** | Beautiful component library |
| **next-themes** | Dark/light mode management |
| **Lucide Icons** | Modern icon set |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance Python API |
| **LangGraph** | Adaptive learning loop orchestration |
| **OpenAI GPT-4.1-mini** | Structured content generation |
| **Pydantic v2** | Data validation and schemas |
| **jsonschema** | JSON validation for AI outputs |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase Postgres** | Persistent learning data (schema: `learnlab`) |
| **pgvector** | Vector embeddings for RAG retrieval |
| **Upstash Redis** | Job queue & caching |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting |
| **Railway** | Backend API |

---

##User Guide

### Getting Started

1. **Create Learner Profile** — Start by creating a learner profile on the dashboard
2. **Select Learning Track** — Choose a track (e.g., "JavaScript Fundamentals")
3. **Run Diagnostic** — Take an initial assessment to identify knowledge gaps
4. **Study Generated Lesson** — Review the personalized lesson with exercises
5. **Take Practice Quiz** — Complete the adaptive quiz and receive detailed feedback
6. **Track Progress** — Monitor mastery updates and follow recommendations

### Understanding Your Learning Journey

| Component | What It Does |
|-----------|--------------|
| **Diagnostic** | Initial assessment to identify skill gaps |
| **Adaptive Lesson** | RAG-generated content targeting your weak areas |
| **Practice Quiz** | Assessment with questions tailored to your level |
| **Mastery Scores** | Per-skill proficiency tracking (0.0–1.0) |
| **Recommendations** | Intelligent suggestions for next learning steps |
| **Analytics** | Comprehensive progress visualization |

### Pro Tips

- **Complete diagnostics first** for accurate gap analysis
- **Review lesson exercises** before taking quizzes
- **Check analytics regularly** to track skill improvement
- **Use the chat assistant** for clarification during lessons
- **Maintain learning streaks** for consistent progress

---

## 🎨 Architecture Highlights

### Recommendation Logic
- **Mastery-Based Gap Analysis** — Identifies skills with lowest proficiency scores
- **Priority Weighting** — Considers skill dependencies and learning paths
- **Adaptive Suggestions** — Recommendations update in real-time based on performance

### Pedagogy-Aware Content Generation
- **RAG-Enhanced Lessons** — Vector search retrieves relevant content chunks
- **Progressive Difficulty** — Exercises and questions adapt to learner level
- **Structured Outputs** — JSON schemas ensure pedagogical consistency
- **Context-Aware Feedback** — Detailed explanations tied to specific skills

### Polished Learning UX
- **State-Driven Interface** — Smooth transitions without page reloads
- **Mobile-First Design** — Responsive with 44px+ touch targets
- **Dark/Light Mode** — System preference support with smooth transitions
- **Accessibility** — WCAG-compliant with proper ARIA labels

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Lesson Generation | ~15-25 seconds |
| Quiz Generation | ~10-20 seconds |
| Frontend Bundle | Optimized with Next.js |
| Mobile Ready | ✅ Yes (9/10 score) |
| Lighthouse Score | 90+ |

---

## 🛡️ Security

- ✅ **RPC-Based Database Access** — Secure Supabase access without exposing schema
- ✅ **API Rate Limiting** — 20 requests/minute per IP
- ✅ **CORS Protection** — Configured for Vercel frontend
- ✅ **Environment Variables** — All secrets stored securely
- ✅ **Input Validation** — Pydantic schemas for all API inputs
- ✅ **Content Safety** — Educational content only, no disallowed categories

---

## 👨‍💻 Creator

**Derril Filemon**

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — LangGraph orchestration, OpenAI structured generation, RAG
- ⚛️ **Modern React** — Next.js 16, React 19.2, Server Components, TypeScript
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic validation
- 🎨 **UI/UX Design** — Responsive design, accessibility, dark/light themes
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔧 **DevOps** — CI/CD, environment management, database migrations
- 📊 **Data Modeling** — Mastery tracking, recommendation algorithms
- 🎓 **Pedagogy** — Adaptive curriculum design, learning analytics

---

## 🙏 Acknowledgments

- **[LangGraph](https://langchain-ai.github.io/langgraph/)** — Multi-node state machine orchestration
- **[OpenAI](https://openai.com/)** — GPT-4.1-mini for structured content generation
- **[Supabase](https://supabase.com/)** — PostgreSQL database with pgvector
- **[Upstash](https://upstash.com/)** — Redis caching and job queue
- **[Railway](https://railway.app/)** — Backend deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful component library

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">


Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
