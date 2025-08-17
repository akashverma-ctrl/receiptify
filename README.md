---

# Receiptify

Receiptify is a lightweight application that simplifies the student registration process by generating digital receipts. It uses **FastAPI** for the backend and a simple **HTML/JavaScript frontend** for form submission. The backend takes student details, fills a `.docx` template, converts it to PDF, and emails the receipt instantly.

---

## Features

* Collects student details via frontend form.
* Generates **PDF receipts** from a `.docx` template.
* Sends receipt automatically to the student’s email.
* Stores data locally in JSON/YAML/Excel for records.
* Easy to run and deploy.

---

## Project Structure

```
Receiptify/
│── backend/
│   ├── recipt_generator.py   # FastAPI backend
│   ├── requirements.txt      # Dependencies
│   ├── template.docx         # Receipt template
│── frontend/
│   ├── index.html            # Form UI
│   ├── script.js             # Handles form submit
│── README.md
```

---

## How to Run Locally 🚀

### 1. Clone the repository

```bash
git clone https://github.com/your-username/receiptify.git
cd receiptify
```

### 2. Set up the backend

```bash
cd backend
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows
pip install -r requirements.txt
```

### 3. Start the backend server

```bash
python recipt_generator.py
```

This will start FastAPI on `http://127.0.0.1:8000`.

### 4. Run the frontend

* Go to the `frontend` folder.
* Open `index.html` in your browser.
* Fill the form → Submit → Receipt will be generated & emailed.

---

## Tech Stack

* **Backend:** FastAPI, Python
* **Frontend:** HTML, JavaScript
* **Document Handling:** python-docx, docx2pdf
* **Emailing:** SMTP

---

## Future Enhancements

* Add authentication for admin dashboard.
* Deploy backend on cloud (e.g., AWS/Heroku).
* Add database support (MySQL/Postgres).

---
