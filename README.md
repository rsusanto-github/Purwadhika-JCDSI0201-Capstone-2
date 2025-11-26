# Corridor Performance Analysis

This Python program analyzes public transport corridor performance using trip data. It computes key metrics, identifies top and bottom performing corridors, and provides insights for operational improvements. The program also supports grouping corridors based on demand and efficiency.

---

## **Features**

* **Data Cleaning & Preparation**

  * Convert timestamps to datetime
  * Calculate trip duration in minutes
  * Extract trip date, hour, and weekday
  * Flag free rides and weekend trips

* **Feature Engineering**

  * Corridor-level aggregation of:

    * Total trips, average, median, and standard deviation of trip duration
    * Total and average revenue per trip
    * Unique passengers, free rides, and ratios
    * Average trips per day
    * Peak hours
    * Revisit rate (returning passengers)
    * Visit variance (stability)
    * Performance score (combines volume and efficiency)

* **Corridor Grouping**

  * Classify corridors into:

    * High Demand – High Efficiency
    * High Demand – Low Efficiency
    * Medium Demand – Medium Efficiency
    * Low Demand – Low Efficiency
  * Summary of group metrics for business insights
  * Suggested operational strategies per group

* **Visualization**

  * Top 10 and bottom 10 corridor performance charts
  * Rainbow color palette for readability
  * Bar charts for total trips, average duration, and performance score

* **Insights**

  * Identifies high-demand corridors and peak hours
  * Highlights revenue vs usage discrepancies
  * Suggests optimization opportunities for low-demand or inefficient corridors

---

## **Dependencies**

* Python 3.8+
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Scikit-learn (for MinMaxScaler)

Install dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## **Usage**

1. **Load your dataset**:

```python
import pandas as pd
df = pd.read_csv("corridor_trip_data.csv")
```

2. **Run the program** to:

   * Compute features
   * Calculate performance metrics
   * Group corridors
   * Generate top/bottom 10 charts
   * Display insights

3. **View results**:

   * `corridor_features` dataframe for all metrics
   * Visualizations for top/bottom performing corridors

---

## **File Structure**

```
corridor_analysis/
├── corridor_analysis.py      # Main program
├── corridor_trip_data.csv    # Input dataset
├── README.md                 # Documentation
└── visuals/                  # Generated charts (optional)
```

---

## **License**

This project is licensed under the MIT License.

---

## **Author**

Robert Susanto

---

## **Contact**

Email: [robert.susanto@example.com](mailto:robert.susanto@example.com)
LinkedIn: [linkedin.com/in/robertsusanto](https://linkedin.com/in/robertsusanto)
