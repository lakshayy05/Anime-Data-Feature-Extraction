# Anime Data Feature Extraction 🎬

A data processing project focused on **Feature Engineering** and extraction using Python and Pandas. This notebook demonstrates how to parse unstructured text strings to create structured, analyzable datasets from raw Anime records.

The project takes a raw dataset (`anime.csv`) where metadata like episode counts and broadcast dates are embedded inside the 'Title' string, and extracts them into clean, numerical columns.

## 🚀 Key Features & Techniques

* **Text Parsing & String Manipulation:**
    * Extracted **Episode Counts** by parsing text between parentheses `( )` in the title string.
    * Cleaned data by removing string artifacts (e.g., " eps") and converting types to integers.
* **Date & Time Handling:**
    * Extracted broadcast periods (e.g., "Oct 2006 - Jun 2007") from raw strings.
    * Converted string dates into datetime objects using `datetime`.
    * Calculated the **Total Duration (in Months)** of anime series using `dateutil.relativedelta`.
* **Exploratory Data Analysis (EDA):**
    * Identified the Anime with the **Highest Score**.
    * Analyzed the Top 5 highest-rated series.
    * Discovered the Anime with the **Maximum Episode Count**.

## 🛠️ Tech Stack

* **Language:** Python 3.13.3
* **Libraries:**
    * `pandas` (Data Manipulation)
    * `numpy` (Numerical Operations)
    * `python-dateutil` (Complex date calculations)
* **Environment:** Jupyter Notebook / Google Colab

## 📂 Project Structure

The notebook follows a logical feature engineering workflow:
1.  **Data Loading:** Importing raw `anime.csv` data.
2.  **Feature Extraction (Episodes):** Custom functions using string loops to isolate episode numbers.
3.  **Feature Extraction (Time):** Logic to parse broadcast windows from title suffixes.
4.  **Transformation:** Converting text ranges into calculated numeric duration (Months).
5.  **Analysis:** Querying the enriched dataset to answer specific questions (e.g., "Which anime ran the longest?").

## 💻 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/LakshayGarg/Anime-Feature-Extraction.git](https://github.com/LakshayGarg/Anime-Feature-Extraction.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy python-dateutil
    ```
3.  **Run the Notebook:**
    Open `Feature_Extraction.ipynb` in Jupyter Notebook or Google Colab.
    *(Note: Ensure `anime.csv` is uploaded to the environment)*

## 👤 Author

**Lakshay Garg**
* [GitHub Profile](https://github.com/lakshayy05)

---
*This project focuses on transforming raw, messy text into structured insights—a critical step in the Data Science pipeline.*
