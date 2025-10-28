# Automatic Form Filler AI

## Overview

Automatic Form Filler AI is a Streamlit-based app for automatically filling scanned or digital forms.
It uses OCR, computer vision, and a user-friendly interface to map your data onto form templates and output completed forms.

## Features

- Upload form images (`png`, `jpg`, `jpeg`)
- AI-powered detection of fields/lines/rectangles
- Input details via interface or CSV bulk filling
- Preview and download filled forms
- Batch fill multiple forms and download as a ZIP file

## Technologies Used

- Python 3.7+
- Streamlit (web UI)
- Pillow, OpenCV, numpy, pandas
- PyTesseract (OCR)

## Installation

1. Clone this repo:
    ```
    git clone https://github.com/A4xPraddy/Automatic_Form_Filler_AI.git
    cd Automatic_Form_Filler_AI
    ```

2. Create and activate a virtual environment:
    ```
    python -m venv venv
    .\venv\Scripts\activate      # Windows PowerShell
    source venv/bin/activate    # macOS/Linux
    ```

3. Install dependencies:
    ```
    pip install streamlit pillow pandas numpy opencv-python pytesseract matplotlib
    ```

4. Install [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) and set its path in `main.py`:
    ```
    pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
    ```

## Usage

1. Run the app:
    ```
    streamlit run stream.py
    ```

2. In your browser:
    - Upload a form image
    - Fill out details in the web UI or upload CSV
    - Preview and download the filled form(s)

## Project Structure

AUTOMATIC_FORM_FILLER_MASTER/
│── stream.py
│── main.py
│── fillFile.py
│── fillData.py
│── fillDetails.py
│── get_fields.py
│── line_detect.py
│── rect_detect.py
│── util.py
│── images/
│── tempDir/


## Contributing

Pull requests are welcome. For major changes, please open an issue first.

## License

This project is licensed under the MIT License.

## Credits

Developed by A4xPraddy(PRASAD).

