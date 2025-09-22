# task-1
data cleaning
# 🎬 Netflix Dataset Cleaning  

## 📌 Overview  
This project focuses on **data cleaning and preprocessing** of the Netflix dataset.  
The main objective is to remove duplicates, handle missing values, standardize formats, and prepare the dataset for further analysis or modeling.  

---

## 🛠️ Steps Performed  

1. **Load Dataset**  
   - Loaded the raw Netflix dataset using Pandas.  

2. **Duplicates & Null Handling**  
   - Removed duplicate records.  
   - Dropped rows with missing `show_id` or `title`.  
   - Filled missing categorical values (`director`, `cast`, `country`, `rating`, `duration`) with `"unknown"`.  

3. **Text Cleaning**  
   - Converted all text to lowercase.  
   - Removed extra spaces for consistency.  

4. **Date Standardization**  
   - Converted `date_added` column into a proper `datetime` format (`dd-mm-yyyy`).  
   - Dropped rows with invalid dates.  

5. **Duration Splitting**  
   - Extracted numeric `duration_value` (e.g., `90`) and `duration_unit` (e.g., `min`, `season`).  
   - Filled missing units with `"unknown"`.  

6. **Column Name Standardization**  
   - Converted all column names to lowercase and replaced spaces with underscores.  

7. **Data Type Fixes**  
   - Converted `release_year` and `duration_value` into numeric values.  
   - Dropped rows with invalid or missing release years.  

8. **Final Cleanup**  
   - Removed any remaining invalid rows.  
   - Exported the cleaned dataset to **`cleaned_netflix.csv`**.  

---

## 📂 Repository Structure  


