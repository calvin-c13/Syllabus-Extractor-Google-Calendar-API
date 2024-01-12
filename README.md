# College Course Syllabus Parser with Google Calendar

## Overview

This Python script automates the extraction of essential information from college course syllabuses in PDF format. It detects the course's instruction mode, the presence of labs, quizzes, and exams related to a course, and prompts the user for additional input to compile comprehensive information.

## Prerequisites

Before using this script, make sure you have the following:

1. **Python Installed:**
   - [Download Python](https://www.python.org/downloads/) if not already installed.

2. **Google Developer OAuth Client ID Credentials:**
   - Obtain OAuth client ID credentials and token.json by following instructions from the [Google Calendar API Quickstart](https://developers.google.com/calendar/api/quickstart/python).

3. **Folder with course syllabuses in pdf form**
   - Ensure that all the courses you want to add to Google Calendar are in a single folder and are in pdf form.

4. **Ensure the python script, credentials.json, token.json, and folder containing syllabuses are in the same working directory**
   
## Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/calvin-c13/syllabus-automated-google-calendar.git
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
