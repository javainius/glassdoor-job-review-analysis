# 📊 Employee Retention Deep Dive: 800k+ Glassdoor Reviews Analysis

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-%2309A3D5.svg?style=for-the-badge&logo=spacy&logoColor=white)
![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white) 

**[Glassdoor Job Reviews Dataset](https://www.kaggle.com/datasets/davidgauthier/glassdoor-job-reviews/)**

## 📌 Project Overview
Why do employees leave within their first year, and what makes veterans stay for a decade? This project leverages **Natural Language Processing (NLP)** to analyze over **800,000 free-text Glassdoor reviews**, mapping the evolution of employee priorities across different career stages.

---

## 🛠 Tech Stack

| Category | Tools |
| :--- | :--- |
| **Data Acquisition** | `kagglehub` |
| **Data Manipulation** | `pandas`, `json`, `os` |
| **NLP** | `spaCy` (Lemmatization), `scikit-learn` (N-gram extraction) |
| **Utilities** | `tqdm` (Progress tracking), `collections` (Frequency analysis) |

---

## 🧠 Data Processing Pipeline

1.  **Text Preprocessing:** Raw review data was cleaned and lemmatized using `spaCy` to ensure linguistic accuracy and eliminate noise.
2.  **Feature Extraction:** Generated **bi-grams** and **tri-grams** to capture critical context (e.g., *"work-life balance"*, *"toxic environment"*) that single words often miss.
3.  **Thematic Mapping:** Developed a custom **JSON-based mapping system** to categorize the **Top 300 n-grams** into 6 "Pros" and 5 "Cons" strategic business themes.
4.  **Segmented Analysis:** Filtered data into four distinct segments (**1, 3, 5, and 10-year tenure**) to identify shifting motivations.

---

## 📊 Key Discoveries

* **⚠️ The Early Exit Drivers:** Work-Life Balance and Company Culture are the primary reasons for leaving within the first year. These are the dominant themes in early-career complaints.
* **💸 The "Salary Myth":** Contrary to popular belief, **Compensation** is the least discussed topic across all segments. While salary may attract candidates, it is rarely the primary driver for long-term retention or departure.
* **⚓ People Hold People:** Among company veterans (5+ and 10+ years), **"People & Coworkers"** is the most frequently mentioned positive theme. Connection is the ultimate anchor.

---

## 💡 Strategic Insights

My analysis suggests that companies should shift their focus from financial incentives to **organizational humanness**.

* **Attraction is not driven by salary alone.** It is achieved by propagating and maintaining a culture of genuine human connection.
* **The "Personality" of an organization is its strongest magnet.** The quality of the core team you build initially will dictate the type and personality of talent you attract later.
* **The Human Element:** In today's data-driven world, the human element remains the most significant variable in employee retention.

---

## 🚀 Installation & Usage

### Clone the repository and navigate to the project folder
git clone https://github.com/yourusername/glassdoor-analysis.git
cd glassdoor-analysis

### Install required Python libraries
pip install pandas spacy scikit-learn kagglehub tqdm

### Download the NLP model for spaCy
python -m spacy download en_core_web_sm
