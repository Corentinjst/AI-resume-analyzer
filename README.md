# 📄 AI Resume Analyzer

![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.8-blue?logo=typescript)
![Tailwind](https://img.shields.io/badge/TailwindCSS-4.1-38B2AC?logo=tailwind-css)
![React Router](https://img.shields.io/badge/React%20Router-7.7-orange?logo=react-router)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

> **AI-powered web app** that evaluates a resume against a job posting and provides an **ATS-friendly score** along with **actionable recommendations** to improve the CV.

---

## ✨ Features

- 📤 **Upload** a resume (PDF) and a job description  
- 🧠 **ATS heuristics**: keyword matching, job title alignment, essential sections  
- 📊 **Scoring system** with visual feedback (gauge, badges, cards)  
- 📝 **Improvement suggestions** (missing keywords, formatting tips, section relevance)  
- 🖼️ **PDF preview** powered by pdf.js  
- ⚡ **Modern UI** with React 19, TypeScript, Zustand, and TailwindCSS  

---

## 🗂️ Project Structure

```
+---app
|   |   app.css
|   |   root.tsx
|   |   routes.ts
|   |   
|   +---components
|   |       accordion.tsx
|   |       ats.tsx
|   |       details.tsx
|   |       fileUploader.tsx
|   |       navbar.tsx
|   |       resumeCard.tsx
|   |       scoreBadge.tsx
|   |       scoreGauge.tsx
|   |       scroreCircle.tsx
|   |       summary.tsx
|   |       
|   +---constants
|   |       index.ts
|   |       
|   +---lib
|   |       pdf2img.ts
|   |       puter.ts
|   |       utils.ts
|   |       
|   \---routes
|           auth.tsx
|           home.tsx
|           resume.tsx
|           upload.tsx
|           wipe.tsx
```

---

## ⚙️ Tech Stack

- **Frontend Framework**: React 19 + React Router 7 (SSR mode with `react-router build/serve`)  
- **Language**: TypeScript 5.8  
- **Bundler**: Vite 6  
- **Styling**: Tailwind CSS 4, `tailwind-merge`, `clsx`  
- **State Management**: Zustand 5  
- **File & PDF Handling**: react-dropzone, pdfjs-dist  

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+  

### Installation

```bash
# Clone the repository
git clone https://github.com/Corentinjst/AI-resume-analyzer
cd AI-resume-analyzer

# Install dependencies
npm install

# Start development server
npm run dev
```

### Production

```bash
# Build production bundle
npm run build

# Run with React Router SSR
npm start
```

By default, React Router dev runs on port `5173`. You can set `PORT` for production.

---

## 🧪 Usage Example

1. Go to **Upload** page  
2. Upload a resume (PDF)  
3. Paste a job description  
4. Click **Analyze** → Get a **score**, **gauge visualization**, and **recommendations**  
5. Adjust your CV according to feedback, re-run analysis  

---

## 🔧 Implementation Notes

- **PDF Parsing**: handled via `pdfjs-dist`  
- **Drag & Drop Upload**: powered by `react-dropzone`  
- **State**: managed with Zustand store  
- **Styling**: Tailwind 4 with `clsx` and `tailwind-merge` for conditional classes  
- **Configurable Weights**: all scoring rules live in `app/constants/index.ts`  

---

## 🙌 Credits

- Inspired by the **JavaScript Mastery** tutorial (YouTube).