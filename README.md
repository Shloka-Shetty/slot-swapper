# Slot‑Swapper 🎯

**Slot‑Swapper** is a full‑stack application built with:  
- **Backend**: FastAPI + SQLAlchemy + MySQL (via `pymysql`)  
- **Frontend**: React (with Vite)  

**Purpose:** Swap or manage time slots efficiently, allowing users to allocate, view, and exchange slots with ease.

---

## 🧩 Features

- User authentication (register, login, JWT tokens)  
- CRUD operations for slots  
- Swap functionality to exchange slots between users  
- Interactive frontend interface to manage/view slots  
- Clean and modular codebase for easy maintenance and extension

---

## 🚀 Getting Started

### 1. Prerequisites

- Node.js (v16 or higher recommended)  
- Python (v3.9 or higher recommended)  
- MySQL server running  
- Environment variables set up in `.env` file

### 2. Backend Setup

```bash
cd backend
python -m pip install --upgrade pip
python -m pip install -r requirements.txt

# Create database if not exists:
# CREATE DATABASE slots_db;

# Start backend server
python -m uvicorn main:app --reload --port 8000


Once running, visit: http://127.0.0.1:8000/docs for API documentation.

3. Frontend Setup
cd frontend
npm install
npm run dev


Frontend should be served at: http://localhost:5173/

4. Environment Variables (.env)

In backend/.env, add:

DB_USER=root
DB_PASSWORD=your_mysql_password
DB_HOST=127.0.0.1
DB_PORT=3307         # or 3306 if you used default
DB_NAME=slots_db

SECRET_KEY=your_super_secret_random_key_here
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=60

🧱 Project Structure
/backend
  ├─ main.py
  ├─ database.py
  ├─ models.py
  ├─ .env
/frontend
  ├─ src/
      ├─ App.jsx
      ├─ components/
      ├─ services/
  ├─ package.json
  ├─ vite.config.js


(Adjust to match actual structure)

🔧 Usage

Register a new user via the API or frontend.

Create, view, edit slots or whatever items your app manages.

Use the swap‑feature: “explain how swapping works briefly”.

Frontend interacts with backend on http://127.0.0.1:8000.

📝 Notes

Ensure MySQL user root has proper permissions on slots_db.

If running MySQL on a non‑default port (3307) ensure .env matches.

Frontend dependencies: react‑router‑dom, axios etc. Ensure they are installed.

✅ License

This project is licensed under the MIT License
