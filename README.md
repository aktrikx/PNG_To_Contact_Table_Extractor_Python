# PNG To Contact Table Extractor Python
This project focuses on automating the extraction of structured contact information from PNG images that contain contact tables. These tables typically include details such as contact name, job title, phone number, extension, email, and role type. The core objective was to convert these often messy and inconsistently formatted image-based tables into a clean, organised Excel file, with one contact per row and all fields correctly aligned.

The problem arose when using traditional OCR tools like Adobe Acrobat, which exported the text but produced unreliable results—data fields were frequently misaligned, with names, titles, and emails appearing on the wrong lines or merged together. Additionally, the variation in field labelling and inconsistent formats for phone numbers and extensions made manual cleanup tedious and inefficient, especially when dealing with multiple image files.

<img width="1433" alt="pngtoexcel_result" src="https://github.com/user-attachments/assets/f7455d73-dafd-4dd9-ad11-111dc5bfbe48" />

To solve this, I developed a Python script that uses Tesseract OCR to extract raw text from each image and applies a combination of regular expressions and logical rules to identify and clean up the relevant data. The script intelligently parses through the OCR output to extract structured information such as names, titles, phone numbers, email addresses, and role types. It uses contextual cues and keyword matching to fix misplacements and inconsistencies. After extracting and organizing the data, the script compiles everything into a structured Excel spreadsheet using the pandas and openpyxl libraries.

The project leverages Python along with libraries such as Pillow for image processing, pytesseract for OCR, pandas for data manipulation, and regular expressions for pattern matching. The result is an efficient, automated pipeline that transforms folders of contact table images into a single, well-formatted Excel file, saving hours of manual data entry and cleanup.

This project demonstrates practical applications of OCR, text processing, and automation, and highlights the power of Python in solving real-world data extraction problems.
