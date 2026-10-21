# Zomato Restaurant Data Analysis (EDA)

##  Project Overview
An Exploratory Data Analysis (EDA) and Data Cleaning pipeline built using **Python, NumPy, and Pandas** to analyze restaurant trends, pricing tiers, and customer rating behaviors.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas (Data Cleaning & Aggregation), NumPy (Statistical Analysis & Vectorized Feature Engineering)

##  Key Data Cleaning & Feature Engineering Steps
1. **Duplicate Removal:** Identified and removed duplicate restaurant entries.
2. **String Parsing & Type Conversion:** Cleaned messy string ratings (`'4.7/5'`, `'NEW'`, `'-'`) and formatted currency strings (`'1,000'`) into numerical floats.
3. **Missing Value Imputation:** Imputed missing ratings using `np.nanmedian()` and missing costs using `np.nanmean()` to prevent outlier skew.
4. **Vectorized Categorization:** Used `np.select()` to classify restaurants into *Budget*, *Mid-Range*, and *Luxury* tiers.

##  Key Business Insights
* **Online Delivery Impact:** Restaurants offering online delivery receive significantly higher customer engagement (votes) compared to offline-only outlets.
* **Location Hubs:** Koramangala and Indiranagar emerge as the highest-density restaurant hubs with strong average ratings (>4.4).
* **Pricing Distribution:** 90% of restaurants fall under the ₹1,800 cost-for-two threshold, making mid-range casual dining the dominant market segment.

##  How to Run the Project
1. Clone the repository:
 
   git clone [https://github.com/apuravbhaskar2005-ux/Zomato-data-analysis.git](https://github.com/apuravbhaskar2005-ux/Zomato-data-analysis.git)
2. Install dependencies:
  pip install pandas numpy
3. Run the script:
  python zomato_analysis.py
