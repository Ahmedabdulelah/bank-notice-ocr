# 📄 Bank Notice OCR

A smart web application that extracts key data (amount & date) from bank notification images using OCR, and logs the results automatically into an Excel sheet.

---

## 💡 Project Idea

This project allows a user to:
1. Upload a bank notification image (receipt, message, etc.).
2. Extract the **amount** and **date** using OCR (Optical Character Recognition).
3. Display the extracted data clearly on the page.
4. Automatically save the data into a pre-existing Excel file for record-keeping.

---

## ⚙️ Technologies Used

| Technology        | Purpose                                           |
|------------------|---------------------------------------------------|
| Python           | Core programming language                         |
| Flask            | Web server and routing                            |
| Tesseract OCR    | Extract text from images (Arabic + English)       |
| Pillow (PIL)     | Image preprocessing to improve OCR accuracy       |
| Regex (re)       | Extract amount and date from plain text           |
| OpenPyXL         | Excel automation (data entry, formatting)         |
| HTML + CSS       | Web page structure and styling                    |
| Bootstrap 5      | Responsive UI design                              |
| JavaScript       | UX enhancement (showing selected file name)       |

---

## 📂 Project Structure

bank-notice-ocr/
│
├── app.py # Main Flask app
├── templates/
│ ├── index.html # Upload form
│ └── result.html # Results display page
├── uploads/ # Temporary image storage
├── إشعارت بنكك.xlsx # Excel file to be updated
└── README.md # This file



---

## 🚀 How to Run

1. **Install Tesseract OCR:**
   - Windows: [Download from here](https://github.com/tesseract-ocr/tesseract)
   - Set the path in `app.py`:
     ```python
     pytesseract.pytesseract.tesseract_cmd = r'C:\\Path\\To\\tesseract.exe'
     ```

2. **Install the required libraries:**
   ```bash
   pip install flask pillow openpyxl pytesseract


3. **Run the app:**
python app.py










