# 📄 ATS Resume Checker

A Streamlit app that scores a resume for ATS (Applicant Tracking System) compatibility using Google's **Gemini 2.5 Flash** model and suggests concrete improvements.

## Features
- Upload a resume as **PDF or DOCX**
- ATS score (0-100) with a 5-category breakdown
- Optional **job description** for a job-match score and missing keywords
- Strengths, weaknesses, prioritized improvements and bullet-point rewrites
- Quick rule-based checks (email, phone, sections, numbers, length)
- Download the report as JSON

## Run locally
```bash
git clone https://github.com/<your-username>/ats-resume-checker.git
cd ats-resume-checker
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Get a free API key at https://aistudio.google.com/apikey, then either:

- paste it into the app's sidebar, **or**
- copy `.streamlit/secrets.toml.example` to `.streamlit/secrets.toml` and put your key in it, **or**
- set an environment variable `GEMINI_API_KEY`.

```bash
streamlit run app.py
```

## Deploy on Streamlit Community Cloud
1. Push this repo to GitHub (never commit your API key).
2. Go to https://share.streamlit.io and sign in with GitHub.
3. Click **Create app**, pick your repo, branch `main`, main file `app.py`.
4. Open **Advanced settings → Secrets** and add:
   ```toml
   GEMINI_API_KEY = "your-key-here"
   ```
5. Click **Deploy**.

## Notes
- Scanned/image-only resumes can't be read; use a text-based PDF or DOCX.
- The ATS score is an AI estimate, not the output of any real ATS.
- Resume text is sent to the Gemini API. Don't upload data you aren't comfortable sharing.
