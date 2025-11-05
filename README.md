<div align="center">

<h1>✨ Binsight AI</h1>
  <h3>Smart Waste Classifier • No Hardware • Built for India</h3>
  <p>An AI-powered web app that identifies plastic, paper, metal, and more from waste images — with zero cloud dependency.</p>
  
 ![Binsight_1](https://github.com/user-attachments/assets/c631360f-0515-4bc6-8bc1-d643173293a3)


  

  <a href="#-local-installation">
    <img src="https://img.shields.io/badge/Local_Setup-MongoDB%20%2B%20FastAPI%20%2B%20React-0056D2?style=for-the-badge&logo=github"/>
  </a>


</div>

---

## 🌍 Why Binsight?

In Ahmedabad, **only 35% of households segregate waste properly** — contaminating recyclables and overloading landfills.

**Binsight** solves this with pure software:
- 📸 **Upload or capture** waste images via browser
- 🤖 **AI classifies** into 6 categories: `cardboard`, `glass`, `metal`, `paper`, `plastic`, `trash`
- 💬 **Rule-based chatbot** answers disposal queries
- 👨‍💼 **Admin dashboard** to review predictions & retrain model
- 🛠️ **100% local**: Runs on your machine — **no cloud, no login, no external APIs**

Built as a **Minor Project** by B.Tech IT students under **Prof. Naimish Patel**.

---

## 🧠 Tech Stack

| Layer        | Technology                     |
|--------------|--------------------------------|
| **Frontend** | React 19 + Tailwind CSS        |
| **Backend**  | Node.js + Express              |
| **AI/ML**    | FastAPI + TensorFlow (Inception) |
| **Database** | MongoDB (local instance)       |
| **Auth**     | JWT (admin only)               |
| **File Upload** | Multer + PIL + OpenCV (via FastAPI) |

> ✅ Entirely **open-source** and **free to run** on your laptop.

---

## 🚀 Local Installation

### Prerequisites
- Node.js v18+
- Python 3.9+
- MongoDB (running locally)
- Git

### Step-by-Step Setup

```bash
# 1. Clone the repo
git clone https://github.com/your-username/binsight-s4f.git
cd binsight-s4f

# 2. Start MongoDB (in a separate terminal)
mongod

# 3. Set up AI Service (FastAPI)
cd ai-service
pip install -r requirements.txt
python index.py  # Runs on http://localhost:8000

# 4. Set up Backend (Node.js)
cd ../backend
npm install
npm start  # Runs on http://localhost:5000

# 5. Set up Frontend (React)
cd ../frontend
npm install
npm start  # Runs on http://localhost:3000
