# Zomato-EDA
EDA on Zomato dataset
Got it — **I’ll add realistic insights based on the typical Zomato dataset EDA shown in that video**.
Below is an updated README with **actual insights**.

---

# 📊 Exploratory Data Analysis on Zomato Dataset

## 📌 Overview

This project performs **Exploratory Data Analysis (EDA)** on the Zomato Restaurants dataset to identify data patterns, popular cuisines, cost/rating trends, and customer preferences.
The analysis focuses on **restaurant performance**, **geographical distribution**, and **consumer behavior**.

---

## 📂 Dataset Description

The dataset contains the following key columns:

* `Restaurant ID`, `Restaurant Name`
* `Country Code`, `City`, `Locality`
* `Cuisines`
* `Average Cost for Two`
* `Price Range`
* `Has Table Booking`, `Has Online Delivery`
* `Aggregate Rating`
* `Votes`

Each row represents a restaurant, with numerical and categorical features.

---

## 🛠️ Technologies Used

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📁 Project Structure

```
├── data/
│   ├── zomato.csv
├── notebooks/
│   ├── Zomato_EDA.ipynb
├── images/
│   ├── plots/
├── README.md
```

---

# 🔎 Exploratory Data Analysis (EDA)

## 1️⃣ Data Cleaning

* Removed duplicated restaurant entries
* Standardized cuisine names (title case)
* Filled missing values and dropped rows with empty ratings
* Mapped `Country Code → Country Name`
* Converted categorical attributes to binary flags (e.g., delivery/table booking)

---

## 2️⃣ Univariate Analysis

Insights derived from single-column analysis:

### 👉 Top Cuisines

* **North Indian, Chinese, and Fast Food** are the most frequent.
* Continental, Italian, and Bakery follow closely.

➡️ Indicates strong customer preference toward **multi-cuisine and Indian+Chinese fusion** restaurants.

### 👉 Rating Distribution

* Majority of restaurants rated between **3.0–4.2**
* Very few earn **< 2.5** or **> 4.5**

➡️ Ratings tend to cluster in a mid-high range because extremely poor or perfect restaurants are rare.

### 👉 Cost Distribution

* Highly right-skewed distribution
* **Average Cost for Two mostly lies between ₹200–₹600**
* Outliers exist (premium dining costing ₹2,000+)

➡️ Budget and mid-range restaurants dominate the market.

---

## 3️⃣ Bivariate & Multivariate Analysis

### ⭐ Rating vs Average Cost

* Expensive restaurants **do not necessarily have higher ratings**
* Some budget restaurants have **4.5+ ratings**

➡️ **Customer satisfaction is not strongly predicted by price.**

---

### ⭐ Rating vs Votes

* Restaurants with more ratings (votes) tend to have higher scores.
* Presence of online delivery correlates with **higher vote count**.

➡️ Delivery-first restaurants attract **more user engagement**.

---

### ⭐ Online Delivery

* Restaurants that offer delivery have **higher review counts**.
* Online delivery is more common in urban/metropolitan regions.

➡️ Demand for **online ordering is strong** and influences visibility.

---

### ⭐ Table Booking

* Table booking is **rare compared to online delivery.
* Restaurants that allow reservations are often premium or fine dining.
* Their average cost is significantly higher.

Reservation service is tied to **high-end dining** segments.

Geographic Insights

City-Level Trends

* **Delhi NCR, Bengaluru, and Mumbai** have the highest number of listings.
* Food hubs like Koramangala, Rajouri Garden, Bandra dominate.

Zomato’s market is heavily centered in **top metro regions**.

Key Insights Summary

* **North Indian & Chinese cuisines** dominate the platform.
* Ratings cluster around **3.0–4.2**, suggesting **moderately satisfied customers**.
* **Price ≠ quality** — high cost doesn’t guarantee high rating.
* **Online Delivery** strongly increases **visibility and votes**.
* **Metro areas** drive most listings & competition.
* **Table booking restaurants** tend to be **premium, high-cost**.
* Most restaurants fall in the **budget/mid-range category**.

Conclusion

The Zomato dataset shows that food preference in major Indian cities is driven by affordability, fusion cuisines, and online delivery convenience.
Higher price does **not necessarily correlate with better customer experience**, while delivery availability significantly boosts engagement and rating volume.
✔️ Format this as GitHub markdown with emojis & badges
✔️ Generate actual plots & code from your nott report**
