# Web Scraping Project

## 📌 Project Overview
This project demonstrates how to perform **web scraping** using Python to extract structured data from an HTML page.  
The target HTML page for this task is:  
**[https://baraasalout.github.io/test.html](https://baraasalout.github.io/test.html)**  

The goal is to extract data from different types of HTML elements and store them in CSV or JSON files for further processing.

---

## 🛠 Steps Performed

### 1. Extract Text Data
- Extracted all **headings** (`<h1>`, `<h2>`).
- Extracted all **text content** inside `<p>` and `<li>` tags.
- **Output:** `Extract_Text_Data.csv`

---

### 2. Extract Table Data
- Extracted **Product Name**, **Price**, and **Stock Status** from the HTML table.
- **Output:** `Extract_Table_Data.csv`

---

### 3. Extract Product Information (Cards Section)
- Extracted:
  - Book Title
  - Price
  - Stock Availability
  - Button Text (e.g., `"Add to basket"`)
- **Output:** `Product_Information.json`

---

### 4. Extract Form Details
- Extracted:
  - Field Name (`name` attribute)
  - Input Type (`type` attribute)
  - Default Value (if any)
- **Output:** `Form_Details.json`

---

### 5. Extract Links and Multimedia
- Extracted **video link** from the `<iframe>` tag.
- **Output:** `Media_Links.json`

---

### 6. Scraping Challenge – Featured Products
- Extracted:
  - Product ID (`data-id` attribute)
  - Product Name 
  - Price 
  - Available Colors 
- **Example Output:**
```json
[
    {"id": "101", "name": "Wireless Headphones", "price": "$49.99", "colors": "Black, White, Blue"},
    {"id": "102", "name": "Smart Speaker", "price": "$89.99", "colors": "Grey, Black"},
    {"id": "103", "name": "Smart Watch", "price": "$149.99", "colors": "Black, Silver, Gold"}
]
