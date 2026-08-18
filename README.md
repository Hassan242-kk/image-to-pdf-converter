# Image to PDF Converter

A simple desktop application built with Python that allows users to select multiple images and convert them into a single PDF file.

## Features

* Select multiple images at once
* Supports PNG, JPG, and JPEG images
* Display selected images in the application
* Enter a custom PDF name
* Choose where to save the generated PDF
* Automatically scales and centers images on PDF pages
* Creates one PDF page for each selected image
* Shows success and error messages

## Technologies Used

* Python
* Tkinter
* Pillow
* ReportLab

## Project Structure

```text
image-to-pdf-converter/
│
├── app.py
├── README.md
└── .gitignore
```

## Requirements

Make sure Python 3.13 or later is installed.

The project uses the following Python packages:

```text
Pillow
ReportLab
```

Tkinter is used for the graphical user interface.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/image-to-pdf-converter.git
cd image-to-pdf-converter
```

### 2. Create a virtual environment

```bash
python3.13 -m venv venv
```

### 3. Activate the virtual environment

On macOS/Linux:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install Pillow reportlab
```

## Run the Application

After activating the virtual environment, run:

```bash
python app.py
```

## How to Use

1. Open the application.
2. Click `Select Images`.
3. Select one or multiple images.
4. Enter the desired PDF name.
5. Click `Convert to PDF`.
6. Choose the location where you want to save the PDF.
7. The application will create the PDF with one image per page.

## How It Works

The application uses Tkinter to create the graphical interface.

Pillow is used to open and process the selected images.

ReportLab is used to create the PDF and place each image on a separate page.

The application calculates the image dimensions and scales each image so that it fits inside the PDF page while maintaining its original aspect ratio.

## Future Improvements

Possible improvements include:

* Drag and drop images
* Remove selected images
* Reorder images
* Choose different PDF page sizes
* Add image rotation
* Add PDF compression
* Add a progress bar
* Create a standalone executable application

## License

This project is available for educational and personal use.
