# AI Resume Analytics App 🤖📄

An AI-powered Resume Analytics application that analyzes resumes, extracts key insights, and helps evaluate candidate profiles using NLP and Machine Learning techniques.

---

## 🚀 Features

- Resume upload (PDF / DOCX)
- Resume parsing using NLP
- Skill extraction & keyword matching
- Resume analytics and scoring
- Job–resume relevance insights
- Bonus resume-writing resources (YouTube integration)
- MySQL database integration
- Secure file handling

---

## 🛠️ Tech Stack

- **Python 3.10+**
- **Flask**
- **MySQL**
- **PyMySQL**
- **NLTK / spaCy**
- **scikit-learn**
- **yt-dlp** (for YouTube video metadata)
- **HTML / CSS / Bootstrap**

---

## 📂 Project Structure
AIResumeAnalyticsApp/
│
├── App.py
├── README.md
├── .gitignore
├── uploaded_resumes/ # ignored by git
├── templates/
├── static/
├── models/
└── requirements.txt


---

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/AIResumeAnalyticsApp.git
cd AIResumeAnalyticsApp


2️⃣ Create virtual environment
python -m venv venv
venv\Scripts\activate   # Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Configure MySQL

Create a MySQL database

Update database credentials in App.py

pymysql.connect(
    host='localhost',
    user='kaify',
    password='your_password',
    database='cv'
)

5️⃣ Run the application
streamlit run App.py

🔐 Security Notes

Uploaded resumes are excluded from version control

Database credentials should be moved to .env for production

Do not commit personal resume data

📈 Future Improvements

Resume ranking using deep learning

Job description matching

Admin dashboard with analytics

Export resume reports (PDF)

Cloud deployment (AWS / Azure)

👨‍💻 Author

Muhammad Kaif ur Rehman
Data Scientist | AI & NLP Enthusiast

⭐ If you like this project

Give it a ⭐ on GitHub and feel free to contribute!


