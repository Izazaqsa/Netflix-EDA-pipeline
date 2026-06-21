#  Netflix Data Exploration & Insights Pipeline

Have you ever wondered how Netflix's library has evolved over the years, or whether they prioritize Movies over TV Shows? 

This project is a deep dive into Netflix's global content catalog. Using **Python**, **Pandas**, and **Matplotlib**, I built a complete Exploratory Data Analysis (EDA) pipeline that transforms messy, missing raw media data into clean, visually striking, and actionable media insights.

---

##  Key Features

Here is exactly what this notebook achieves step-by-step:

###  Real-World Data Cleaning
* **Smart Missing Value Handling:** Instead of just throwing away incomplete rows, I categorized missing directors and actors as `'unknown'`.
* **Advanced Time-Series Interpolation:** For missing upload dates (`date_added`), I implemented **linear interpolation** to smoothly estimate data points based on surrounding trends instead of deleting them.
* **Data Typofixes:** Formatted text dates into actual `datetime` objects and isolated anomalies (like duration data accidentally mixed into the rating column).

###  Creative Feature Engineering
* **Seasonality Tracking:** I extracted the exact month each title was added and mapped it to a specific season (Winter, Spring, Summer, Autumn) to check if Netflix drops more content during specific quarters of the year.

###  Rich Data Visualizations
* **Content Split:** A clear breakdown comparing the total volume of Movies vs. TV Shows.
* **Release Trends:** Line charts showing how platform content additions have grown exponentially over the last decade.
* **Seasonal Releases:** A colorful pie chart visualizing which seasons see the heaviest content drops.

---

##  Tech Stack & Tools

* **Language:** Python 3.x
* **Data Wrangling:** Pandas & NumPy
* **Data Visualization:** Matplotlib 
* **Environment:** Jupyter Notebook / VS Code Virtual Environments (`venv`)

---

##  Project Structure

```text
├── netflix-project.ipynb   # The main Jupyter Notebook containing all cleanups, code, and charts
├── netflix_titles.csv      # Raw dataset containing over 8,000+ rows of Netflix history
└── README.md               # This project documentation
