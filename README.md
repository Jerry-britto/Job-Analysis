# Job Postings Data Analysis: Summary and Insights

## 📌 Project Workflow
The analysis followed a structured data analysis workflow:

1. **Problem Definition**  
   Address skill/location-based job searches and salary compensation.

2. **Data Exploration & Cleaning**  
   Examine dataset quality and perform necessary cleaning steps.

3. **Data Analysis & Visualization**  
   Extract and visualize key insights to answer market-related questions.

4. **Summary**  
   Consolidate findings into a clear overview.

---

## 🔍 Data Exploration and Cleaning

- **Dataset Overview**  
  - **Total job postings:** 79,147  
  - **Features:** 12 (e.g., job role, company, experience, salary, location)  

- **Issues Identified**  
  - **Missing Values:**  
    - Rating & Reviews: ~36,000 missing entries each  
    - Experience & Location: Some missing entries  
  - **Duplicate Entries:** Over 6,000 duplicates (based on `job_id`)  
  - **Irrelevant Information:**  
    - Columns removed: `posted_on`, `job_link`, `company_link`

- **Cleaning Steps**  
  1. Dropped rows with critical missing information (e.g., `job_id`, `company`)  
  2. Filled missing `experience` and `location` with most frequent values  
  3. Imputed missing `rating` with mean company rating  
  4. Removed duplicate job postings  
  5. Engineered **min_experience** and **max_experience** from the experience column  
  6. Converted `reviews` column to numerical format  

---

## 📊 Key Findings and Analysis

- **Final Dataset Size:** 72,967 unique job postings from 15,310 unique companies

### 🏢 Top Companies by Job Postings
1. Lavya Associates  
2. Accenture  
3. Hucon  
4. Varite India Pvt. Ltd.  
5. IBM  

### 💡 Most In-Demand Skills
- Focused heavily on **sales** and **communication** roles.  
- **Top 10 Skills:**
  1. Sales  
  2. Communication  
  3. Agency  
  4. Tied  
  5. Customer Service  
  6. Training  
  7. Team Handling  
  8. Javascript  
  9. Agency Channel  
  10. Java  

### 🎯 Skills for Specific Roles and Companies
- **Data Scientist Roles:**  
  - Machine Learning  
  - Python  
  - Deep Learning  
  - NLP  
  - Data Science  

- **HDFC Bank Roles:**  
  - Portfolio Management  
  - Cross-Selling  
  - Sales  
  - Relationship Management  

---
