# PDF Question Answering Web App (Using AI)

This is a simple web application built with Django that allows users to upload a PDF file and ask questions about its content. The application extracts text from the PDF and uses OpenAI's GPT model to generate answers based on the content.

## Features

- **PDF Upload:** Users can upload a PDF file through a web form.
- **Question Answering:** After uploading the PDF, users can ask questions about its content.
- **OpenAI Integration:** The app uses OpenAI's GPT model to generate answers from the extracted PDF text.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x
- Django 3.x or higher
- An OpenAI API key

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/pdf-qa-app.git
   cd pdf-qa-app

2. **Create and activate a virtual environment:**
   
   ```bash
   python3 -m venv venv
   source venv/bin/activate


3. **Install the required packages:**
    
    ```bash
    pip install -r requirements.txt

4. **Set up your OpenAI API key:**
   
   ```bash
   Open settings.py and add your OpenAI API key:
   OPENAI_API_KEY = 'your-openai-api-key'

5. **Run the Django development server:**

   ```bash
   python manage.py migrate
   python manage.py runserver

6. **Access the application:**
   
   ```bash
   Open your web browser and go to http://127.0.0.1:8000/.

	 Upload a PDF and ask a question:
	 Upload a PDF file using the provided form.
	 Enter a question related to the PDF content.
	 Submit the form to get an answer generated by the OpenAI GPT model.
 
7. **Project Structure**

   ```bash
		<pre>
		```markdown
		pdf_qa/
		│
		├── pdf_qa/                   # Main project directory
		│   ├── __init__.py
		│   ├── settings.py           # Django settings
		│   ├── urls.py               # URL configuration
		│   ├── wsgi.py
		│   └── asgi.py
		│
		├── qa_app/                   # Main app directory
		│   ├── __init__.py
		│   ├── admin.py
		│   ├── apps.py
		│   ├── forms.py              # Form for PDF upload and question submission
		│   ├── models.py
		│   ├── tests.py
		│   ├── urls.py               # App-specific URL configuration
		│   ├── utils.py              # PDF text extraction and OpenAI interaction
		│   ├── views.py              # Main view handling the PDF upload and QA
		│   └── templates/qa_app/     # HTML templates
		│       ├── upload.html       # Form for uploading PDF and asking a question
		│       └── result.html       # Display the answer
		│
		├── manage.py                 # Django management script
		└── requirements.txt          # Python dependencies
		```
		</pre>


8. **Dependencies**

```bash
	•	Django
	•	PyMuPDF (fitz)
	•	OpenAI API



<img width="586" alt="Screenshot 2024-08-12 at 11 48 33 PM" src="https://github.com/user-attachments/assets/a8ede71d-cdde-4e9e-a858-fe06300707d5">


