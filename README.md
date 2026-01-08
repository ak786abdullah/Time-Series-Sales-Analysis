# Time Series Sales Analysis

##  Overview
This project is a **Time Series Analysis** script built with **Python** and **Pandas**. It simulates daily sales data for a retail scenario and performs statistical analysis to identify trends, smooth out volatility, and aggregate revenue over specific time periods.

As a Mathematics graduate transitioning into Data Science, I built this project to demonstrate practical applications of **temporal data manipulation**, **rolling statistics**, and **resampling techniques**.

##  Technologies Used
* **Python 3.x**
* **Pandas:** For time-series manipulation, indexing, and aggregation.
* **NumPy:** For data simulation and array handling.

##  Key Features
1.  **Data Simulation:** Generates realistic mock sales data for January 2025 using NumPy.
2.  **Temporal Indexing:** Utilizes Pandas `DatetimeIndex` to enable powerful time-based slicing and operations.
3.  **Trend Analysis (Smoothing):** Calculates a **3-Day Rolling Average** to smooth out daily sales fluctuations and reveal underlying trends.
4.  **Aggregation (Resampling):** Resamples daily data into **Weekly Revenue Totals** (`'W'` frequency) to analyze high-level performance.
5.  **Peak Detection:** Automatically identifies the specific date with the highest recorded revenue.

##  How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/time-series-sales-analysis.git](https://github.com/yourusername/time-series-sales-analysis.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy
    ```
3.  **Run the script:**
    Open `Time Series Sales Analysis.ipynb` in Jupyter Notebook or VS Code and run all cells.
## Key Learnings:
​Mastered pd.to_datetime and set_index to handle time-series data effectively.
​Learned the difference between Rolling Windows (moving averages) and Resampling (grouping by time).
​Applied mathematical concepts (statistics) to business data contexts.


##  Sample Output
The script generates insights similar to the following:

```text
--- Daily Sales & Moving Averages (First 5 Days) ---
            Revenue  3_Day_Moving_Avg
Date                                 
2025-01-01      499               NaN
2025-01-02      398               NaN
2025-01-03      367        421.333333

--- Weekly Revenue Totals ---
2025-01-05    1868
2025-01-12    1921
...

Highest Sales occurred on: 2025-01-15
