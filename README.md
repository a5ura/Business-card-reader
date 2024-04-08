"Business Card Text Extractor

This Python-based tool effortlessly scans images of business cards to capture and store essential contact details. By processing any provided business card image, 
the script efficiently extracts textual information, such as names, phone numbers, and email addresses, making them readily available in a text file for easy access and storage.

## How It Works

The script employs OpenCV for initial image preprocessing, enhancing the clarity and readability of the text. Following this, Tesseract-OCR is utilized to perform
Optical Character Recognition (OCR) on the image, transforming the visual data into a string of text. The extracted text is then parsed to identify
key pieces of information - specifically, email addresses and phone numbers are extracted using regular expressions, and the entire extracted content is saved to a file.

## Getting Started

### Prerequisites

Before running the script, ensure that you have Tesseract-OCR installed on your system, along with Python's OpenCV and pytesseract libraries.

- Install Tesseract-OCR:
  - Windows: Download and install from the Tesseract at UB Mannheim page.
  - Linux: Use `sudo apt-get install tesseract-ocr`.
  - macOS: Use `brew install tesseract`.

- Install Python dependencies:
  ```bash
  pip install opencv-python pytesseract
  ```

### Configuration

If Tesseract-OCR is not recognized by the script, you may need to specify the path to the Tesseract executable in your system. This can be done by setting the `pytesseract.pytesseract.tesseract_cmd` variable in the script.

### Running the Script

1. Clone or download this repository to your local machine.
2. Place the business card image you wish to scan in a known directory.
3. Modify the `image_path` variable in the script to point to your image file.
4. Execute the script. The extracted information will be saved in a file named `extracted_info.txt` in the same directory as the script.

## Note

The script's efficiency in extracting text accurately depends heavily on the quality of the business card image and its complexity. Adjustments to image preprocessing may be necessary for optimal text recognition.

## License

This project is open-sourced under the MIT License. See the LICENSE file for more details."
