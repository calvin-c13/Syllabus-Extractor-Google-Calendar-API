# Automatic College Course Syllabus Parser with Google Calendar

## Overview

This Python script automates the extraction of essential information from college course syllabuses in PDF format.

**Example PDF:**
- [Stony Brook University CS Syllabus](https://syllabus.stonybrook.edu/sites/default/files/courses/cse101/fall-2020/01-lec/cse101-01-fall-2020-syllabus.pdf)

It detects the course's name, the instruction mode, the presence of labs, quizzes, and exams related to a course, and prompts the user for additional input to compile comprehensive information.

## Prerequisites

Before using this script, make sure you have the following:

1. **Python Installed:**
   - [Download Python](https://www.python.org/downloads/) if not already installed.

2. **Code Editor and Google Email Account:**
   - A code editor (such as VS Code) and a working Google Email account.

3. **Google Developer OAuth Client ID Credentials:**
   - Obtain OAuth client ID credentials and `token.json` by following instructions from the [Google Calendar API Quickstart](https://developers.google.com/calendar/api/quickstart/python).
   - Replace the scope in `quickstart.py` with `SCOPES = ["https://www.googleapis.com/auth/calendar"]` (remove `readonly`).

4. **Folder with Course Syllabuses in PDF Form:**
   - Ensure all courses to add to Google Calendar are in a single folder and in PDF form.

5. **Set Up the Working Directory:**
   - Ensure the Python script, `credentials.json`, `token.json`, and the folder containing syllabuses are in the same working directory.

   
## Usage (In terminal)

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/calvin-c13/Syllabus-Extractor-Google-Calendar-API.git
   cd syllabus-automated-google-calendar
2. **Create virtual environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate

3. **Install Required Modules**
   ```bash
   pip install pdfminer.six google-auth google-auth-oauthlib google-auth-httplib2
   pip install google-api-python-client
   pip install --no-binary :all: charset_normalizer
4. **Run the Python Script**
   ```bash
   python3 main.py
