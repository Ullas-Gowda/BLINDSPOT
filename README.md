# BLINDSPOT

# Private Personas - Privacy-First Marketing Extension

A browser extension that enables ethical, transparent, and privacy-preserving personalization using user-controlled personas instead of surveillance-based targeting.

---

## 🚀 MVP Features

* Persona selection UI (user chooses intent like "Eco-shopper", "Budget Traveler")
* Personalized ad recommendation based on persona (not user identity)
* "Why this ad?" button with explainable AI logic
* All user data stored locally (no cookies, no tracking)
* Optional backend for analytics (aggregated, non-identifiable)

---

## 🧱 Tech Stack

### Frontend (Browser Extension)

* HTML, CSS, JavaScript
* React.js (optional)
* Chrome Extension Manifest V3
* LocalStorage or IndexedDB

### Backend (Optional for demo)

* FastAPI (Python)
* SQLite or JSON-based store
* Dummy persona-to-ad matcher
* Anonymized feedback logger

### ML/AI (for matching logic & explainability)

* Rule-based mapping (MVP)
* Future-ready for: LightGBM, SHAP, TF Lite

---

## 📁 Folder Structure

```
private-personas-extension/
├── extension/
│   ├── popup.html / popup.jsx
│   ├── popup.css
│   ├── popup.js
│   ├── manifest.json
│   ├── background.js
│   └── explainability.js
├── backend/
│   ├── main.py (FastAPI)
│   ├── routes/
│   └── models/
├── data/
│   └── persona_tags.json
├── advertiser-portal/
│   └── React-based mock dashboard
├── scripts/
│   └── simulate_feedback.py
├── README.md
```

---

## 🧠 How It Works

1. User installs the extension.
2. On any site, they can pick personas from the extension popup.
3. Ads shown are tagged to personas (not individuals).
4. User can click "Why this ad?" to see reasoning.
5. No personal data is stored or shared.
6. (Optional) Ad performance data is logged in anonymized format for brand insights.

---

## 🛠️ Installation

**Extension**

1. Clone this repo
2. Go to `chrome://extensions/`
3. Enable Developer Mode
4. Click "Load Unpacked" → Select `/extension` folder

**Backend (if demoing)**

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## 📊 Future Features

* Federated model training
* Advanced explainable AI (LIME/SHAP)
* Persona feedback learning loop
* Cross-site persona sync (privacy-compliant)

---

## 🧑‍💻 Team

* \[Member 1] – Frontend, UX, Explainability
* \[Member 2] – Backend, ML, Data Pipeline

---

## ⚖️ License

MIT License
