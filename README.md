# Resume ATS Scoring System

## Description

This project is a Flask-based web application that evaluates resumes against job descriptions using an ATS (Applicant Tracking System) scoring mechanism. It utilizes NLP techniques with the Sentence-BERT model to compute the semantic similarity between a resume and a job description. The application also checks for relevant industry-specific keywords and provides suggestions for improvement.

## Features

- Upload resumes in PDF, DOCX, or TXT formats.
- Upload job descriptions in PDF, DOCX, or TXT formats.
- Compute an ATS score based on semantic similarity.
- Identify industry-specific keywords present in the resume.
- Suggest missing keywords to improve ATS compatibility.
- Caching mechanism to optimize repeated computations.
- Flask web interface with API endpoints.

## Technologies Used

- **Flask** - Web framework for building the application.
- **SentenceTransformers** - Pre-trained Sentence-BERT model for text similarity.
- **LangDetect** - Language detection for input validation.
- **PyPDF2 & docx2txt** - Libraries for text extraction from PDF and DOCX files.
- **Flask-Caching** - Caching mechanism to improve performance.

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/aqibfirdous/resume-ats-scoring.git
   cd resume-ats-scoring
   ```

2. Create a virtual environment (optional but recommended):

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install dependencies:

   ```sh
   pip install -r requirements.txt
   ```

## Usage

1. Start the Flask server:

   ```sh
   python app.py
   ```

2. Open the application in your browser:

   ```sh
   http://127.0.0.1:5000/
   ```

3. Upload a resume and job description, then view the ATS score and suggestions.

## API Endpoints

- **`POST /ats_score`** - Upload resume and job description files to receive an ATS score.

## Contributing

Feel free to submit issues, pull requests, or suggestions to improve the project.

## License

This project is licensed under the MIT License.

## Author

Aqib Firdous

