# 🎬 Netflix Content Strategy Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Libraries](https://img.shields.io/badge/Library-Pandas%20|%20Seaborn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## 📌 Executive Summary
This project performs a comprehensive Exploratory Data Analysis (EDA) on Netflix's content catalog (2021). The goal is to uncover trends in content strategy, specifically focusing on the shift from Movies to TV Shows, global production hotspots, and the "vintage" lag between theatrical release and streaming addition.

**Key Insight:** Netflix has drastically reduced the time lag for acquiring newer content, showing a pivot toward "Fresh" releases over legacy libraries.

---

## 📊 Key Findings

### 1. The "TV Show" Pivot
While Movies still make up the majority of the catalog (**~69%**), the rate of TV Show additions has accelerated significantly since 2016. This aligns with the "Binge-Watching" era strategy.

### 2. Duration Optimization
* **Movies:** The median duration is **90-100 minutes**. However, there is a significant cluster of short-duration content (<60 mins), likely documentaries and specials.
* **TV Shows:** Most shows are canceled or conclude after **1 Season**, indicating a high turnover rate in content experimentation.

### 3. Geographical Dominance
The United States leads production, but **India** and the **United Kingdom** show distinct content profiles. India is heavily skewed toward Movies, whereas the UK and South Korea have a stronger balance of TV content.

---

## 🛠️ Methodologies

### Data Cleaning Pipeline
* **Imputation:** Handled missing values in `director`, `cast`, and `country` using mode and logical placeholders.
* **Type Casting:** Converted `date_added` to datetime objects and extracted temporal features (`year_added`, `month_added`).
* **Feature Engineering:**
    * `duration_minutes`: Extracted integers from mixed string formats.
    * `years_to_netflix`: Calculated the lag between content release and platform addition.

### Visualizations
* **Univariate:** Histograms (Release Year), KDE Plots (Duration).
* **Bivariate:** Correlation Heatmaps, Box Plots (Rating vs. Duration).
* **Multivariate:** Grouped Bar Charts (Top Countries by Content Type).

---

## 📈 Visual Highlights

| Content Distribution | Vintage Analysis |
|:---:|:---:|
| *[Insert your Pie Chart here]* | *[Insert your Scatter Plot here]* |
| *Movies vs. TV Shows dominance* | *Correlation between Release Year & Added Year* |

*(Note: Images are generated dynamically in the notebook)*

---

## 💻 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Netflix-Content-Strategy-Analysis.git](https://github.com/YOUR_USERNAME/Netflix-Content-Strategy-Analysis.git)
