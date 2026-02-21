# 🍒 Zenith Journal

## Basic Details
**Team Name:** ZENITH

### Team Members
- **Niranjana Menon** — Muthoot Institute Of Technology And Science  
- **Tanmaya Remeyn** — Muthoot Institute Of Technology And Science  

### Hosted Project Link
[Add deployed link / GitHub Pages / Vercel / Netlify]

---

## 🧠 Project Description
Zenith Journal is an emotionally intelligent journaling web app that detects harmful thought patterns **while the user is writing** and gently intervenes before emotional spirals intensify.

Instead of analyzing emotions after writing, the system monitors behavioral and linguistic signals in real time and provides grounding, reframing, and breathing interventions.

---

## ❗ The Problem
Most mental wellness and journaling apps are passive — they help only **after** a person has already spiraled into distress.

People experiencing anxiety or rumination often:
- Repeat negative thoughts unconsciously
- Escalate emotions rapidly while writing
- Realize harmful thinking only after emotional damage

There is currently no tool that actively interrupts unhealthy thinking patterns **during the moment they happen**.

---

## 💡 The Solution
Zenith Journal continuously analyzes writing behavior and language patterns to detect cognitive distortions in real time.

When distress increases, the app intervenes using psychology-backed techniques:
- Reflection prompts at moderate distress
- Guided breathing cycle at high distress
- AI-generated gentle reframes after writing

The app acts like a thinking support companion — not just a diary.

---

## ⚙️ Technical Details

### Technologies/Components Used

#### Software

**Languages**
- JavaScript
- Python
- HTML/CSS

**Frameworks**
- React (Vite)
- FastAPI

**Libraries**
- Groq SDK
- React Router DOM
- dotenv
- MongoDB

**Tools**
- VS Code
- Git & GitHub


#### Hardware
_Not applicable_

---

## ✨ Features

**Spiral Meter**  
Real-time emotional intensity score based on typing behavior, repetition, and negative phrasing.

**Reframe Gym**  
Temporarily locks the journal and prompts reflective thinking at moderate distress levels.

**Breathing Orb (Spiral Mode)**  
Guided breathing intervention when emotional intensity crosses critical threshold.

**AI Distortion Detection**  
LLM analyzes entries and suggests gentle reframes.

**Cognitive Fingerprint**  
Tracks recurring thinking patterns locally and privately.

**Crisis Detection**  
Detects high-risk phrases and shows helpline resources non-intrusively.

---

## 🚀 Implementation

### Installation
```bash
git clone https://github.com/tanmayarem/Zenith_Journal.git
cd Zenith_Journal
npm install

cd backend
python -m venv venv
venv\Scripts\activate
pip install fastapi uvicorn groq python-dotenv
```

### 🚀 Run

### Backend
```bash
cd backend
venv\Scripts\activate
uvicorn main:app --reload --port 8000
```

### Frontend
```bash
npm run dev
```

Open http://localhost:5174

---

## 🏗 System Architecture

Frontend (React)  
→ collects behavioral signals  
→ calculates intensity score  
→ sends entry to backend  

Backend (FastAPI)  
→ sends text to Groq LLM  
→ detects distortions  
→ returns reframing suggestions  

Database (MongoDB)  
→ stores journal entries and cognitive fingerprints
→ enables long-term pattern tracking

---

## 🔌 API Documentation

**Base URL:** `http://localhost:8000`

### POST /analyze
Analyze journal text for cognitive distortions

#### Request
```json
{
  "text": "I always ruin everything"
}
```

#### Response
```json
{
  "distortions": ["overgeneralization", "self_blame"],
  "reframe": "Making one mistake doesn't define you."
}
```

---

## 📸 Screenshots
<img width="1907" height="866" alt="Screenshot 2026-02-21 092304" src="https://github.com/user-attachments/assets/1fd1e82b-d937-45e3-96a8-c2903fbe2a20" />
<img width="1877" height="864" alt="Screenshot 2026-02-21 091054" src="https://github.com/user-attachments/assets/307c16de-dffe-4cbc-a261-9c4d0754203a" />
<img width="1887" height="882" alt="Screenshot 2026-02-21 091152" src="https://github.com/user-attachments/assets/d0f4936a-a66e-419a-ab1b-964d168acc71" />
<img width="1887" height="880" alt="Screenshot 2026-02-21 091336" src="https://github.com/user-attachments/assets/4b5946f4-7101-4057-be63-937b61ed3baa" />
<img width="1868" height="857" alt="Screenshot 2026-02-21 091349" src="https://github.com/user-attachments/assets/017eef41-e9d0-4129-8295-a19f902e202f" />
<img width="1880" height="858" alt="Screenshot 2026-02-21 091405" src="https://github.com/user-attachments/assets/246252a7-0c49-42ee-bca1-31666680e78e" />

- Editor with spiral meter
- Reframe intervention
- Breathing orb mode

---

## 🎥 Project Demo


Shows:
- Real-time spiral detection
- Intervention triggers
- AI reframe feedback

---

## 🤖 AI Tools Used
**Tool:** Claude
**Purpose:** debugging, prompt design, architecture planning  


### Human Contributions
- UX & psychology mapping
- Scoring logic design
- Behavior tracking implementation
- Intervention experience design

---

## 👥 Team Contributions
**Niranjana Menon:** Backend API, AI integration 

**Tanmaya Remeyn:** Frontend behavior system, scoring logic, UI/UX , database

---

## 📄 License
This project is licensed under the **MIT License** — see the `LICENSE` file for details.


---

Made with ❤️ at **TinkerHub**
