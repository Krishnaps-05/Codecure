# MedGuard: AI Hallucination Detection for Medical Chatbots

MedGuard is a cutting-edge full-stack application designed to make medical AI safer. It implements a **Dual-Layer Verification System** to detect hallucinations and risky medical claims in AI-generated responses.

## 🚀 Features

- **Primary Chatbot:** Generates detailed medical information.
- **Hallucination Detection Layer (HDL):**
  - **Rule-based Audit:** Scans for high-risk keywords (dosage, surgery, etc.) and missing disclaimers.
  - **Knowledge Validation:** Cross-references answers against a curated collection of verified medical facts.
  - **Confidence Scoring:** Assigns a reliability score (0-100) to every response.
- **Visual Safety Branding:** 
  - 🟢 **Safe:** High confidence, consistent with known facts.
  - 🟡 **Uncertain:** Moderate confidence, potential for ambiguity.
  - 🔴 **High Risk:** Detected hallucination or dangerous lack of disclaimers.
- **Premium UI:** Futuristic healthcare dashboard with glassmorphism, smooth animations, and responsive design.

## 🛠️ Tech Stack

- **Frontend:** React (Vite), Framer Motion, Lucide Icons, Axios.
- **Backend:** FastAPI (Python), Pydantic.
- **AI Logic:** Hybrid Rule-Engine + Knowledge Dataset.

## 📁 Project Structure

```text
├── backend/
│   ├── main.py            # FastAPI Entry Point
│   ├── requirements.txt   # Backend Dependencies
│   └── model/
│       ├── detector.py    # Hallucination Detection Logic
│       └── dataset.json   # Verified Medical Facts
├── frontend/
│   ├── src/
│   │   ├── components/    # React Components (Chat, Message, Badge)
│   │   ├── App.jsx        # Main App Component
│   │   └── index.css      # Design System & Styling
│   └── package.json       # Frontend Dependencies
└── README.md
```

## ⚙️ Setup Instructions

### Backend Setup
1. Navigate to the backend folder: `cd backend`
2. Install dependencies: `pip install -r requirements.txt`
3. Start the server: `python main.py` or `uvicorn main:app --reload`

### Frontend Setup
1. Navigate to the frontend folder: `cd frontend`
2. Install dependencies: `npm install`
3. Start the dev server: `npm run dev`

## ⚠️ Disclaimer
**MedGuard is a prototype for demonstration purposes only.** It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.

---
*Verified by MedGuard AI*
