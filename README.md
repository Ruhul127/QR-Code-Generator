
# QR Code Generator

## Overview

The **QR Code Generator** is a web application built with **Flask**, **Python**, **HTML**, **CSS**, and **JavaScript**. This application allows users to input a URL, generate a QR code for it, and download the QR code as a PNG image.

> Below is an example QR code generated by this project, directing users to YouTube:

![QR Code Example](QR_code_generator/assets/qr-code-example.PNG)

---

## Features

- **Generate QR Codes**: Input any valid URL to receive its QR code.
- **Downloadable Output**: Save the generated QR code as a PNG file with a single click.
- **Responsive Design**: The user interface is optimized for all screen sizes and devices.

---

## Project Structure

The project is organised as follows:

```plaintext
qr-code-generator/
├── app.py                   # Flask application script
├── templates/
│   └── index.html           # HTML template for the user interface
├── static/
│   └── style.css            # CSS file for styling
├── assets/
│   └── qr-code-example.PNG  # Example QR code image
```

---

## Getting Started

### Prerequisites

Ensure the following are installed on your system:

- **Python 3.7+**
- **Pip** (Python package manager)

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/qr-code-generator.git
   cd qr-code-generator
   ```

2. **Set Up a Virtual Environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application**:
   ```bash
   python app.py
   ```

5. Open your browser and navigate to `http://127.0.0.1:5000`.

---

## Usage Instructions

1. Launch the application in your web browser.
2. Enter a valid URL in the input field.
3. Click the **"Generate QR Code"** button.
4. View the generated QR code displayed below the input form.
5. Use the **"Download QR Code"** button to save the image to your device.

---

## Technical Details

### Backend: Flask

The backend is implemented in Flask and provides the following functionality:

- **`/generate` Endpoint**:
  - Accepts POST requests with the URL in JSON format.
  - Uses the `qrcode` Python library to generate the QR code.
  - Returns the generated QR code as a downloadable PNG image.

### Frontend: HTML, CSS, JavaScript

- **HTML**: Defines the structure of the web page, including the form and QR code display area.
- **CSS**: Ensures the application has a clean, responsive design.
- **JavaScript**:
  - Manages form submissions without reloading the page.
  - Displays the generated QR code and provides a download link dynamically.

---
