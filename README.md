# 🍽️ Zomato Restaurant Data Analysis Using Python

A **comprehensive exploratory data analysis (EDA)** project on Zomato restaurant data aimed at uncovering **patterns, trends, and relationships** in restaurant ratings, pricing, cuisines, and services.
The project leverages Python’s data analysis ecosystem to provide **actionable insights** into the food and restaurant landscape across major cities and countries.

---

## 📋 Table of Contents

* [🎯 Goals of the Project](#-goals-of-the-project)
* [📊 Dataset Overview](#-dataset-overview)
* [🛠️ Libraries Used](#️-libraries-used)
* [💡 Key Business Questions](#-key-business-questions)
* [⚙️ Project Workflow](#️-project-workflow)
* [📈 Important Visualizations](#-important-visualizations)
* [🔍 Key Findings & Insights](#-key-findings--insights)
* [💻 Installation & Usage](#-installation--usage)
* [📁 Project Structure](#-project-structure)
* [🚀 Future Improvements](#-future-improvements)

---

## 🎯 Goals of the Project

* Clean and explore the Zomato restaurant dataset for better interpretability.
* Analyze **factors influencing restaurant ratings and popularity.**
* Identify **dominant cuisines, price patterns, and service features**.
* Derive **data-backed insights** for improving restaurant recommendations and business strategy.

---

## 📊 Dataset Overview

* **Source:** Zomato Restaurants Dataset (Kaggle)
* **Records:** 9,551 (approx.) restaurants
* **Features:** 21 (Demographics, Pricing, Cuisine, Ratings, and Services)
* **Target Variable:** `Aggregate Rating`
* **Missing Values:** Present in multiple columns; handled using imputation and cleanup.
* **Data Cleaning Notes:**
  * Dropped irrelevant columns like `Restaurant ID`, `Locality`, `Longitude`, `Latitude`, `Currency`, and `Country Code`.
  * Converted service flags (e.g., `Has Table booking`, `Is delivering now`) to numeric for analysis.

---

## 🛠️ Libraries Used

| Library                  | Purpose                                             |
| ------------------------ | --------------------------------------------------- |
| **NumPy**                | Numerical computations and matrix operations        |
| **Pandas**               | Data cleaning, manipulation, and feature extraction |
| **Matplotlib / Seaborn** | Visualizations and trend analysis                   |
| **Plotly (optional)**    | Interactive charts                                  |
| **Warnings / OS**        | Performance optimization and code readability       |

---

## 💡 Key Business Questions

1. What are the **top cuisines** dominating the Zomato dataset?
2. How do **price range and ratings** correlate?
3. Which **cities and countries** have the most restaurants listed?
4. How do **online delivery and table booking** features affect restaurant ratings?
5. How are **votes, price range, and average cost** distributed across restaurants?
6. What do **customer rating trends** reveal about restaurant quality?

---

## ⚙️ Project Workflow

1. **Data Loading & Cleaning**
   * Imported dataset and handled missing values.
   * Dropped irrelevant columns and standardized categorical values.

2. **Feature Engineering**
   * Converted binary categorical columns into numerical form.
   * Grouped cuisines and price ranges for easier visualization.

3. **Exploratory Data Analysis (EDA)**
   * Examined distributions of numerical features (`Average Cost`, `Votes`, `Aggregate Rating`).
   * Identified top cuisines and city dominance.
   * Analyzed relationships between features using scatter plots and heatmaps.

4. **Insights & Summary Generation**
   * Extracted meaningful business insights from visual trends and correlation patterns.

---

## 📈 Important Visualizations

| Visualization                 | Key Insight                                                           |
| ----------------------------- | --------------------------------------------------------------------- |
| **Cuisines Bar Chart**        | North Indian and Chinese dominate the cuisine landscape.              |
| **Country-wise Distribution** | India contributes ~90.7% of the restaurants; Turkey the least.        |
| **City-wise Count Plot**      | New Delhi tops the list, followed by Gurgaon and Noida.               |
| **Rating Distribution**       | 43% of restaurants have ratings between 2.6–3.5; very few exceed 4.6. |
| **Votes Distribution**        | 91% of restaurants have 0–500 votes — most are less famous.           |
| **Price Range vs Rating**     | Higher price range correlates with slightly higher ratings.           |
| **Online Delivery vs Rating** | Online delivery ensures moderate ratings (3–4 range).                 |
| **Table Booking vs Rating**   | Table booking shows consistent moderate-to-high ratings.              |

---

## 📈 Visual Insights


### 🍜 Top Cuisines
<img src="images/top_cuisines.png" alt="Top Cuisines" width="1000">

### 🌍 Country Distribution
<img src="images/country_distribution.png" alt="Country Distribution" width="1000">

### 🌍 City Distribution
<img src="images/city_distribution.png" alt="City Distribution" width="1000">

### ⭐ Rating Distribution
<img src="images/rating_distribution.png" alt="Rating Distribution" width="1000">

### 💸 Price Range vs Rating
![Price Range vs Rating]([https://github.com/Strik3r10/Zomato-EDA/blob/main/images/rating_vs_price.png?raw=true](https://github.com/Strik3r10/Zomato-Restaurant-EDA/blob/main/Images/pr_rating.png))

### 🧾 City vs Price Range
<img src="images/city_pr.png" alt="City vs Price Range" width="1000">

### 🧾 Country vs Price Range
<img src="images/country_pr.png" alt="Country vs Price Range" width="1000">


## 🔍 Key Findings & Insights

* 🍛 **Top Cuisines:** North Indian and Chinese dominate, followed by Fast Food, Mughlai, and Café.
* 🏙️ **Geographic Insights:**
  * New Delhi, Gurgaon, and Noida host the majority of listings.
  * India accounts for **90.7%** of all restaurants.
* 💬 **Ratings:**
  * Most ratings cluster between **3.0–4.0**, indicating average satisfaction.
  * Only **2%** of restaurants achieve ratings above 4.6.
* 💸 **Pricing & Cost:**
  * Majority of restaurants fall in **price range 1–2**, signaling low to mid-tier affordability.
  * “Average Cost for Two” is **right-skewed**, with few high-end outliers.
* 📊 **Votes:**
  * 91.7% of restaurants have **0–500 votes**, revealing a long-tail pattern.
  * Votes and aggregate rating are **positively correlated** — higher votes, higher ratings.
* 🧾 **Services:**
  * Restaurants with **table booking and online delivery** features tend to have better ratings.
  * Restaurants without these features show lower consistency and lower price ranges.

---

## 💻 Installation & Usage

```bash
# Clone the repository
git clone https://github.com/<your-username>/Zomato-Restaurant-EDA.git

# Navigate to the project directory
cd Zomato-Restaurant-EDA

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook "Exploratory Data Analysis of Zomato Restaurants Dataset.ipynb"
```

---

## 📁 Project Structure

```
Zomato-Restaurant-EDA/
│
├── Exploratory Data Analysis of Zomato Restaurants Dataset.ipynb   # Main notebook
├── Insights & Charts.docx                                          # Insight summary document
├── Dataset                                                         # Dataset 
├── Images                                                          # Images
└── README.md                                                       # Readme

```

---

## 🚀 Future Improvements

* 🔮 Implement **predictive models** to forecast restaurant ratings using regression or ML algorithms.
* 🌐 Add **interactive dashboards** using Streamlit, Plotly, or Power BI.
* 📊 Create **geospatial heatmaps** to visualize restaurant density by city or region.
* 🧩 Apply **text analysis** on restaurant names or reviews (if available).
* 💾 Build a **recommendation engine** for users based on cuisine, price, and rating preferences.

---

## ⭐ Acknowledgements

Dataset sourced from **Zomato via Kaggle** for academic and analytical purposes.
Special thanks to open-source contributors of Python data libraries for enabling robust data analysis.

---

## 🧩 Author

**Mohammad Owais Farooqui**  
📧 [owaisf1jc@gmail.com](mailto:owaisf1jc@gmail.com)  
🌐 [GitHub](https://github.com/Strik3r10)
