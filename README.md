# 🏨 Hotel Booking Data Analysis using Python

An in-depth exploratory data analysis of hotel booking data, uncovering cancellation patterns, pricing trends, customer preferences, and actionable business recommendations for City and Resort hotels.

---

## 📌 Project Overview

This project analyzes hotel booking data to understand what drives cancellations, how pricing affects booking behaviour, which countries cancel the most, and what meal types and hotel types guests prefer. The analysis concludes with data-driven business recommendations for hotel management.

---

## 📂 Dataset

- **Source:** [Kaggle — Hotel Booking Demand Dataset](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- **File used:** `hotel_bookings.csv`
- **Key columns:** `hotel`, `is_canceled`, `adr` (Average Daily Rate), `country`, `meal`, `market_segment`, `reservation_status_date`, `is_repeated_guest`

---

## 🧹 Data Cleaning

- Converted `reservation_status_date` to datetime format
- Dropped columns with excessive null values: `company`, `agent`
- Removed rows with remaining null values
- Removed ADR outlier (records where `adr > 5000`)

---

## 🔍 Analysis Breakdown

### ❌ Cancellation Analysis
- Overall cancellation rate — **37%** of all reservations are cancelled
- Bar chart of reservation status count (Cancelled vs Not Cancelled)
- Monthly cancellation trends — **August** has the most cancellations; **January** has the highest cancellation ratio
- Cancellation rate comparison: **City Hotel vs Resort Hotel**

### 🏨 Hotel Type Preferences
- Pie chart — **City Hotels** are more popular than Resort Hotels
- Count plot of reservation status by hotel type
- Resort Hotels face fewer cancellations than City Hotels

### 💰 Average Daily Rate (ADR) Analysis
- Line chart of ADR over time for both City and Resort Hotels
- Resort Hotel prices spike on **weekends and holidays**
- Bar chart of ADR per month for cancelled bookings — confirms **higher price = more cancellations**
- Zoomed-in line chart (2016 to mid-2017) comparing ADR of cancelled vs non-cancelled bookings

### 🍽️ Meal Type Preferences
- Count plot of preferred meal types — **BB (Bed & Breakfast)** is the most popular

### 🌍 Country-wise Cancellations
- Pie chart of top 10 countries by cancellation count
- **Portugal** has the highest cancellation percentage

### 📢 Market Segment Analysis
- Booking distribution across market segments
- Cancellation percentage breakdown by market segment

---

## 💡 Key Insights & Business Recommendations

- 📉 **High prices drive cancellations** — hotels should revisit pricing strategies, especially for specific locations
- 🏖️ **Resort Hotels** should offer weekend/holiday discounts to reduce cancellation gaps
- 📅 **January** campaigns — targeted marketing in January can boost revenue during the highest cancellation month
- 🇵🇹 **Portugal** — improve service quality to reduce the high cancellation rate from Portuguese guests
- 🍳 **Meal variety** — improve meal options beyond BB to improve guest satisfaction and retention

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| Pandas | Data loading, cleaning & manipulation |
| Matplotlib | Bar charts, pie charts & line plots |
| Seaborn | Count plots & statistical visualizations |
| Google Colab | Development environment |

---

## 🚀 How to Run

### Option 1 — Open in Google Colab
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

*(Replace with your actual Colab notebook link)*

### Option 2 — Run Locally
```bash
git clone https://github.com/anshu1516/Hotel-Booking-Data-Analysis.git
cd Hotel-Booking-Data-Analysis

pip install pandas matplotlib seaborn

jupyter notebook Hotel_Booking_Data_Analysis.ipynb
```

> **Note:** Download `hotel_bookings.csv` from Kaggle and place it in the same directory before running.

---

## 👤 Author

**Anshu** — [GitHub](https://github.com/anshu1516)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
