# GitHub API Repository Analysis

## 📌 Project Overview

In this project, I collected and analyzed real-world data from the **GitHub Search API** using Python.  
Instead of web scraping HTML pages, this project uses an official API and works with **JSON data**, which is the recommended and professional approach when an API is available.

The main goal of this project is to practice:
- Working with APIs
- Understanding and parsing JSON data
- Converting raw data into a structured format
- Performing simple data analysis using pandas

This project was developed as part of my learning journey in the  
**IBM Data Science Professional Certificate (Coursera)**.

---

## 🧠 Key Concepts Practiced

- API vs Web Scraping decision-making
- HTTP requests and status codes
- JSON structure (`dict` and `list`)
- Data extraction from nested objects
- Data cleaning
- Basic data analysis (`count`, `mean`, `groupby`)
- Exporting clean data to CSV

---

## 🔍 Data Source

- **GitHub Search API**
- Endpoint used:  
  `https://api.github.com/search/repositories`

The API returns repository data in JSON format, including metadata such as:
- Repository name
- Number of stars
- Programming language
- Repository URL

---

## 📊 Data Collected

For each repository, the following fields were extracted:

- **Repo_Name** – Full name of the repository  
- **Stars** – Number of GitHub stars  
- **Language** – Main programming language  
- **URL** – Repository URL  

---

## 🛠 Tools & Libraries

- Python  
- `requests` – for API requests  
- `pandas` – for data manipulation and analysis  

---

## 🔄 Project Workflow

1. Send a request to the GitHub Search API
2. Check the response status code
3. Parse the JSON response
4. Extract relevant fields from each repository
5. Create a pandas DataFrame
6. Clean missing values
7. Sort repositories by star count
8. Perform simple analysis:
   - Count repositories by language
   - Calculate average stars per language
9. Save results to CSV files

---

## 📁 Project Structure

github-api-repository-analysis/
│
├── github_api_repo_analysis.py
│   # Main Python script:
│   # - Sends request to GitHub API
│   # - Parses JSON response
│   # - Cleans and analyzes data
│   # - Exports results to CSV
│
├── github_repos_sorted.csv
│   # Cleaned and sorted repository data
│
├── github_language_summary.csv
│   # Summary statistics by programming language
│
└── README.md
    # Project documentation
