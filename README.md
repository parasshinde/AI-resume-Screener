I designed and implemented a fully automated AI Resume Screener that ingests candidate resumes and compares them against a curated set of job descriptions. Leveraging the all‑MiniLM‑L6‑v2 transformer model from Hugging Face, the system encodes both resumes and job postings into dense vector representations. By computing cosine similarity scores, it ranks each candidate’s compatibility with available roles.

Key aspects include:

Data Pipeline: Imported and preprocessed resume documents (PDF, DOCX, TXT) and standardized job description text from the Hugging Face dataset.

Embedding & Matching: Utilized the all‑MiniLM‑L6‑v2 model for efficient sentence‑level embeddings, enabling sub-second inference for scoring thousands of resume–job pairs.

Scoring & Ranking: Developed a ranking algorithm that outputs a normalized match score, highlighting top candidates for each position.

User Interface: Created a simple web dashboard where recruiters upload resumes and view ranked results, complete with score breakdowns and keyword matches.

Impact: Reduced manual screening time by over 70%, increased consistency in candidate shortlisting, and provided transparency with explainable match metrics.

Tech Stack: Python, gradio, Hugging Face Transformers, Pandas.
