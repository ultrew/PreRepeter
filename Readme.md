# 📄 PreRepeter – Smart PDF Question Analyzer 🧠

**PreRepeter** is a full-stack web app that helps students analyze multiple previous year question paper PDFs, detect repeated or similar questions, and export them as a clean `.docx` file — ready for focused revision!

> 🚀 Live Demo: [pre-repeter-frontend.vercel.app](https://pre-repeter-frontend.vercel.app)

---

## 📚 Why I Built This

As a student, I always struggled to find **repeated questions** across past years' papers — manually scanning every PDF before exams was time-consuming and painful.  
So, I built PreRepeter to solve that problem once and for all. 🔁

---

## 💡 Features

✅ Upload **multiple PDFs**  
✅ Extracts text using `PyMuPDF`  
✅ Finds **similar/repeated questions** with `RapidFuzz` (AI fuzzy matching)  
✅ 📥 Generates a **.docx file** listing all matched questions  
✅ Simple UI with drag & drop + upload  
✅ Instant download!

---

## 🛠 Tech Stack

### 🔹 Frontend:
- React
- Tailwind CSS
- React Dropzone
- Vite
- ShadCN UI

### 🔹 Backend:
- FastAPI
- PyMuPDF (for text extraction from PDFs)
- RapidFuzz (for fuzzy matching / similarity detection)
- python-docx (to generate .docx files)

### 🔹 Deployment:
- Frontend: [Vercel](https://vercel.com)
- Backend: [Render](https://render.com)

---

## 🚧 Upcoming Features

🛠 These are under development:
- Filter by **minimum question length**  
- Control **similarity threshold**  
- Filter by **keyword(s)**  
- Re-design download button + toast feedback

Stay tuned!

---

## 📸 Screenshots

[https://github.com/ultrew/PreRepeter/blob/ae3f4e26ac56c1d4a3833b1ca0565bd542f285c8/img.png]

---

## 🧪 Running Locally

```bash
# 1. Clone the repo
git clone https://github.com/ultrew/PreRepeter-backend
git clone https://github.com/ultrew/PreRepeter-Frontend

# 2. Setup backend (Python 3.9+)
cd PreRepeter-backend
pip install -r requirements.txt
uvicorn main:app --reload

(open new window)

# 3. Setup frontend
cd PreRepeter-Frontend
npm install
npm run dev

# 4. Open in browser
http://localhost:5173
