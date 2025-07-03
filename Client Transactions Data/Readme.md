```markdown
# 🧽 Client Transaction Data Cleaning (Excel Project)

This project is part of my Excel data cleaning portfolio. It demonstrates step-by-step cleaning and formatting of a raw client transaction dataset using Microsoft Excel.

---

## 📄 Dataset Overview

**Columns in dataset:**
- Date
- Client
- Contact
- Department
- Region (new column created)
- Payment
- Revenue
- Profit
- Profit Margin

---

## 🧹 Cleaning Methods Used

### 🔸 General Cleaning
- **Auto-fit columns and row widths** to enhance visibility and layout

### 🔸 `Client` Column
- Removed extra data enclosed in parentheses using **Find & Replace**
- Converted all entries to lowercase using the `LOWER()` function

### 🔸 `Contact` Column
- Applied `TRIM()` to remove extra spaces
- Used `PROPER()` to standardize name casing (e.g., "john doe" → "John Doe")

### 🔸 `Department` Column
- Used **Text to Columns** to separate **Department** and **Region** into two columns
- Created a new column called `Region` from the split

### 🔸 Duplicates
- Removed duplicate rows using **Remove Duplicates** feature

### 🔸 `Payment` Column
- Filled blank cells with `NA` using:
  - **Find & Select > Go To Special > Blanks**
  - Entered `NA` and used `Ctrl + Enter` to fill all at once

### 🔸 `Profit Margin` Column
- Fixed cells with formula errors using:
  - `=IFERROR(Profit/Revenue, "NA")` to handle division errors

### 🔸 Final Touches
- Formatted header row with bold text and cell coloring for readability

---

## 📁 Files in Folder



'''client\_transactions/
├── raw data.xlsx        # Original uncleaned dataset
├── cleaned data.xlsx    # Final cleaned version
├── README.md                   # This file
'''


---

## ✅ Skills Demonstrated

- Data cleaning using Excel functions and tools
- Text manipulation with formulas
- Handling missing and error values
- Formatting for clarity and presentation
- Creating clean, analysis-ready datasets

---

## 🛠 Tools Used

- Microsoft Excel
- Functions: `LOWER()`, `TRIM()`, `PROPER()`, `IFERROR()`
- Tools: Find & Replace, Go To Special, Remove Duplicates, Text to Columns, Auto-fit formatting

---

> This project is part of my journey to build a strong foundation in data cleaning and Excel-based data analysis.

```
