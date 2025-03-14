# MCQ Generator

## Overview
This project is a **Flask-based MCQ generator** that extracts text from uploaded files (PDF, TXT, DOCX) and generates multiple-choice questions (MCQs) using Google Generative AI.

## Features
- **File Upload Support**: Accepts PDF, TXT, and DOCX files.
- **Text Extraction**: Extracts content from the uploaded document.
- **AI-Generated MCQs**: Uses Google Generative AI to create MCQs from the extracted text.
- **Downloadable Results**: Saves the generated MCQs as a text file and a PDF for download.
- **Web Interface**: Simple UI for uploading files and generating MCQs.

## Requirements
Make sure you have the following installed:
- **Python 3.x**
- **Flask**
- **OpenAI Google Generative AI SDK**
- **pdfplumber** (for extracting text from PDFs)
- **docx** (for handling DOCX files)
- **Werkzeug** (for secure file handling)
- **FPDF** (for generating PDFs)

### Install Dependencies
Run the following command to install the required libraries:
```sh
pip install -r requirements.txt
```

## How to Run the Application
1. Clone or download the project.
2. Open a terminal and navigate to the project directory.
3. Set up the API key for Google Generative AI by setting the environment variable `API_KEY`.
4. Run the Flask application:
   ```sh
   python app.py
   ```
5. Open `http://127.0.0.1:5000/` in your web browser.
6. Upload a file, specify the number of MCQs, and generate.
7. Download the generated MCQs in text or PDF format.

## Folder Structure
```
mcq-generator/
│── templates/          # HTML templates for Flask
│── .gitignore          # Git ignore file
│── app.py              # Main Flask application
│── requirements.txt    # Dependencies
│── README.md           # Documentation
```

## How It Works
- The user uploads a file via the Flask web interface.
- The application extracts text and sends it to Google Generative AI.
- AI-generated MCQs are saved as a text file and a PDF.
- The user can download the results.

## Possible Enhancements
- **Support for More File Types**: Extend compatibility to CSV, PPTX, and images.
- **Customizable MCQ Format**: Allow users to set difficulty levels or specify question styles.
- **Integration with Learning Management Systems**: Export MCQs to LMS-compatible formats.

## License
This project is open-source. Feel free to modify and improve it!

## Author
Biswajit Mallik 
