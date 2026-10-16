# AI-POWERED-RESUME-ANALYSER
# AI-Powered Resume Analyzer

An intelligent resume analysis web application that evaluates resumes against job descriptions, identifies relevant skills, measures job-role compatibility, and provides suggestions to improve resume quality and ATS (Applicant Tracking System) compatibility.

## 🚀 Features

- **Resume Parsing:** Upload resumes in PDF or DOCX format for analysis.
- **Skill Extraction:** Identifies technical skills and compares them with the requirements of a selected job role.
- **Resume–Job Matching:** Uses BERT-based sentence embeddings to measure semantic similarity between resumes and job descriptions.
- **Resume Match Score:** Combines skill matching and semantic similarity to calculate an overall match score.
- **ATS Compatibility Checker:** Evaluates resumes based on skills, experience, projects, education, certifications, and summary.
- **Resume Improvement Suggestions:** Provides recommendations to improve resume content and job relevance.
- **AI-Generated Text Detection:** Integrates a transformer-based detector to estimate whether text may be AI-generated.
- **Interactive Dashboard:** Displays resume analysis results and matching insights.
- **Job Description Dataset:** Uses a curated CSV dataset containing job descriptions for roles such as AI Engineer, ML Engineer, and Data Analyst.

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Web Framework | Flask |
| NLP & Semantic Matching | Sentence Transformers, BERT |
| Embedding Model | `all-MiniLM-L6-v2` |
| AI Text Detection | `Hello-SimpleAI/chatgpt-detector-roberta` |
| Document Processing | PDF and DOCX parsing libraries |
| Data Processing | Pandas, CSV |
| Frontend | HTML, CSS, JavaScript |
| Dataset | `data/job_descriptions.csv` |

## ⚙️ How It Works

1. **Upload Resume:** The user uploads a resume in PDF or DOCX format.
2. **Extract Content:** The application extracts the resume text and relevant information.
3. **Identify Skills:** The skill extraction module identifies technical skills and important keywords.
4. **Match Job Description:** BERT-based embeddings compare the semantic similarity between the resume and the selected job description.
5. **Calculate Match Score:** Skill matching and semantic similarity are combined using configurable weights of 40% and 60%, respectively.
6. **Check ATS Compatibility:** The application evaluates important resume sections and identifies potential areas for improvement.
7. **Display Results:** The dashboard presents the match score, skill insights, ATS checks, and improvement suggestions.

## 📂 Project Structure

```text
AI_Resume_Analyzer/
├── app.py
├── data/
│   └── job_descriptions.csv
├── resume_parser.py
├── skill_extractor.py
├── bert_matcher.py
├── scorer.py
├── ats_checker.py
├── resume_suggestions.py
├── templates/
├── static/
└── requirements.txt
```

*Note: The structure above illustrates the main modules. Actual filenames and folders may vary depending on the project version.*

## 💻 Installation and Setup

### Prerequisites

- Python 3.10 or a compatible version
- pip
- Git

### 1. Clone the repository

```bash
git clone https://github.com/jyothikak05/AI-POWERED-RESUME-ANALYSER.git
cd AI-POWERED-RESUME-ANALYSER
```

### 2. Create a virtual environment

```bash
python3 -m venv venv
```

Activate it on macOS or Linux:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

### 5. Open the application

Visit the following address in your browser:

```text
http://127.0.0.1:5002
```

## 🎯 Objectives

- Simplify the initial resume screening process.
- Help candidates understand how closely their resumes align with job descriptions.
- Identify relevant skills and potential skill gaps.
- Improve resume structure and ATS compatibility.
- Provide actionable, data-driven feedback for job applications.

## 🔮 Future Enhancements

- Integrate more job roles and frequently updated job descriptions.
- Improve skill extraction using advanced NLP techniques.
- Generate personalized resume recommendations for specific job postings.
- Add resume version comparison and downloadable analysis reports.
- Enhance accessibility and the user interface.

## ⚠️ Disclaimer

The resume match score and ATS checks are estimates intended to support resume improvement. They do not guarantee shortlisting or hiring outcomes. AI-generated text detection may produce false positives or false negatives and should not be treated as definitive proof.

## 👩‍💻 Author

**Jyothika Kothakonda**

GitHub: [@jyothikak05](https://github.com/jyothikak05)

---
