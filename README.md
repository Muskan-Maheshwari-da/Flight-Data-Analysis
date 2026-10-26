# ✈️ Flight Data Analysis & Performance Dashboard (Python & Power BI)

An end-to-end data analytics project that cleans and processes raw aviation data using Python, followed by an interactive Power BI dashboard for visualizing flight delays, airline performance, root causes, and airport efficiency.

---

## 🧹 1. Python Data Cleaning & Preprocessing (`Airlines.ipynb`)
In the first phase of this project, raw flight data was thoroughly cleaned, transformed, and prepared for analysis using **Python (Pandas)** inside Jupyter Notebooks. Key steps included:
* **Handling Missing Values:** Identified and treated null or missing records in critical operational columns.
* **Data Type Casting:** Converted date fields (`FlightDate`) to standard datetime formats and ensured numeric metrics (delays, flights) were set to correct integer/decimal types.
* **Feature Engineering & Formatting:** Processed arrival/departure delay metrics (`ArrDelayMinutes`, `DepDelay`), extracted hourly time attributes for trend analysis, and standardized airline/airport codes.
* **Data Export:** Cleaned and optimized the final dataset (`cleaned_flight_data`) to ensure smooth integration with Power BI.

---

## 📊 2. Power BI Interactive Dashboard

### A. Dashboard Preview
![Flight Data Analysis Dashboard](Screenshot%202026-10-25%20211643.png)

### B. Key Features & Visuals
* **Top KPI Cards:** 
  * **Total Flights & Total Delays:** Overall flight volume versus total delay occurrences.
  * **Delay Rate % & Cancellations:** Percentage share of delayed flights and total cancellations.
  * **Avg Arrival Delay:** Average delay duration in minutes.
* **Interactive Slicers:** 
  * `FlightDate` Slicer for timeline filtering.
  * `Reporting_Airline` Slicer configured with a **Filter** for major carriers.
  * `Origin Airport` Slicer for dynamic location-based filtering.
* **Core Analytical Charts:**
  * **A. Airline Performance & Ranking:** Horizontal bar chart comparing delay counts across top airlines.
  * **B. Hourly Delay Trend:** Line/Area chart tracking delay frequencies across hours of the day.
  * **C. Delay Root Causes Breakdown:** Donut chart categorizing delay factors (Carrier, Weather, NAS, Security, Late Aircraft).
  * **D. Top 10 Delayed Airports:** Column chart highlighting airports with the highest record of delays.

---
├── flight.pbix                          # Power BI Dashboard File
├── Screenshot 2026-10-25 211643.png     # Dashboard Visual Preview
└── README.md                            # Project Documentation
