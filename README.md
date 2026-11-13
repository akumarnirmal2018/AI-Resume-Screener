# AI Resume Screener

An AI-powered resume screening system that uses Large Language Models (LLMs) to analyze resumes, extract candidate information, compare candidate skills with job descriptions, and rank candidates based on their suitability for a job role.

## 🚀 Features

- **Job Description Analysis:** Extracts required skills, preferred skills, education requirements, experience requirements, and responsibilities from job descriptions.
- **Resume Parsing:** Extracts candidate information from PDF and DOCX resumes.
- **AI-Powered Evaluation:** Uses Groq LLM to compare resumes with job descriptions.
- **Candidate Matching:** Evaluates candidate skills, experience, and qualifications.
- **Match Score:** Generates an overall candidate matching score (0–100).
- **Candidate Ranking:** Sorts candidates based on their matching scores.
- **Top Candidates:** Identifies the top 2 candidates.
- **Lowest Candidates:** Identifies the 2 lowest-scoring candidates.

## 🛠️ Tech Stack

- **Python**
- **Groq API**
- **Large Language Models (LLMs)**
- **Pydantic** – Data validation and structured outputs.
- **PyPDF** – Extracting text from PDF resumes.
- **Python-docx** – Reading DOCX resumes.
- **JSON** – Structured data handling.
- **Python-dotenv** – Managing environment variables.

## 📂 Project Structure

```text
AI-Resume-Screener/
│
├── resume_folder/
│   ├── resume1.pdf
│   └── resume2.pdf
│
├── LLM_RESUME_EVALUATOR.py
├── pyproject.toml
├── uv.lock
├── .python-version
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/akumarnirnal2018/AI-Resume-Screener.git
```

### 2. Navigate to the Project Directory

```bash
cd AI-Resume-Screener
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install groq pydantic python-dotenv pypdf python-docx
```

### 5. Configure API Key

Create a `.env` file in the project directory:

```env
GROQ_API_KEY=your_groq_api_key
```

Replace `your_groq_api_key` with your actual Groq API key.

### 6. Add Resumes

Place PDF or DOCX resumes inside the `resume_folder` directory.

### 7. Run the Project

```bash
python LLM_RESUME_EVALUATOR.py
```

## 🔄 How It Works

1. The system takes a job description as input.
2. The LLM analyzes the job description and extracts structured requirements.
3. It reads resumes from the resume folder.
4. The resume parser extracts candidate information.
5. The system compares each candidate's resume with the job requirements.
6. It calculates an overall matching score.
7. Finally, candidates are sorted and ranked according to their scores.

## 🔐 Environment Variables

The project requires a Groq API key.

Never upload your `.env` file or API keys to GitHub.

## 🔮 Future Improvements

- Develop a web-based interface using Streamlit or React.
- Support additional resume formats.
- Generate detailed candidate evaluation reports.
- Improve candidate ranking using advanced matching techniques.
- Add database integration to store candidate information.
- Build an interactive recruiter dashboard.

## 👨‍💻 Author

**Avinash Kumar**

GitHub: https://github.com/akumarnirnal2018

---

⭐ If you find this project interesting, consider giving it a star!

