# AI Resume Analyzer 🤖📄

An AI-powered application that parses PDF resumes using Natural Language Processing (NLP) to provide career recommendations, skill gap analysis, and resume scoring. Built for recruiters to visualize data and users to improve their job prospects.

## 🚀 Key Features

* **Automated Parsing:** Extracts name, contact info, and skills using `pdfminer.six` and custom **spaCy** pipelines (Replaced legacy `pyresparser`).
* **Skill Classification:** Categorizes candidates into fields like Data Science, Web Dev, Android, iOS, and UI/UX.
* **Interactive Recommendations:** Suggests specific skills and certificates to boost the candidate's profile.
* **Resume Scoring:** Generates a dynamic score based on the presence of critical resume sections (Objective, Achievements, etc.).
* **Admin Dashboard:** Features a secure login and data visualization (Pie Charts) for analyzed user profiles.
* **Video Integration:** Contextual YouTube videos for resume writing and interview preparation.

## 🛠️ Tech Stack

* **UI/Frontend:** [Streamlit](https://streamlit.io/)
* **NLP Engines:** `spaCy`, `NLTK`
* **Database:** `MySQL` (via `PyMySQL`)
* **Visualization:** `Plotly Express`
* **PDF Extraction:** `pdfminer.six`

## Project Structure

```text
AI-Resume-Analyzer/
├── App.py                # Main Streamlit Application
├── Courses.py            # Course & Video data lists
├── Logo/                 # Static assets (logo2.png)
├── Uploaded_Resumes/     # Temporary storage (gitignored)
├── .streamlit/           # Configuration folder
│   └── secrets.toml      # Database credentials (gitignored)
├── requirements.txt      # Project dependencies
└── README.md             # Documentation
```

## ⚙️ Setup & Installation

### 1. Database Setup
Ensure MySQL is running. Create the database:
```sql
CREATE DATABASE cv;
```

## 2. Clone the repository
```bash
git clone https://github.com/Mkaify/AIResumeAnalyticsApp.git
cd AIResumeAnalyticsApp
```

## 3. Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate  # Windows
# Activate on Mac/Linux:
# source venv/bin/activate
```

## 4. Install dependencies
```bash
pip install -r requirements.txt
```

## 5. Configure Secrets (Crucial)
Create a folder named .streamlit in the root directory and add a file named secrets.toml. Add your database credentials inside:
```Ini, TOML
# .streamlit/secrets.toml
DB_HOST = "localhost"
DB_USER = "root"
DB_PASSWORD = "your_password"
DB_NAME = "cv"
ADMIN_USER = "Mkaify"
ADMIN_PASSWORD = "Mkaify123"
```
## 6. Run App
```bash
streamlit run App.py
```

## 👨‍💻 Author
Muhammad Kaif ur Rehman Software Engineering Student | AI & NLP Enthusiast
