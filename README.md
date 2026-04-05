# Cosmic Origins: NASA Meteorite Landings Analysis ☄️

An interactive Power BI dashboard exploring over 31,000 extra-terrestrial impacts recorded by NASA. This project focuses on data cleaning, geospatial visualization, and temporal analysis to uncover patterns in how and where meteorites strike Earth.

![Project Preview](gif) 

## 📌 Project Overview
The goal of this project was to transform raw NASA data into an intuitive visual story. It provides insights into the mass distribution of meteorites, the frequency of landings over time (860 AD – 2013), and geographical hotspots using a sleek, dark-themed interface.

## 📊 Key Insights & Features
* **Global Impact Heatmap:** A geospatial map categorized by meteorite type (Iron, Stony, Stony-Iron, and Other/Achondrite) with high-density clusters in Europe and North America.
* **Top 10 Heaviest Meteorites:** A dynamic bar chart highlighting the most massive recorded impacts, featuring data labels for immediate value recognition.
* **Temporal Trend Analysis:** A line chart identifying a significant spike in recorded landings during the late 20th century.
* **Key Performance Indicators (KPIs):**
    * **Total Recorded Impacts:** 31.69K+
  
    * **Largest Recorded Meteorite by Impact & Type:**
      * 60,000 kg (Hoba, Iron, Namibia, 1920)
      * 4,300 kg (Brenham, Stony-Iron, USA, 1882)
      * 4,000 kg (Jilin, Stony, China, 1976)
      * 3,000 kg (Al Haggounia 001, Other/Achondrite, Oman, 2006)
     
    * **First Recorded Impact:**
      * 0.47 kg (Nogata, Stony, Japan, 860 AD)

    * **Last Recorded Impact:**
      * 100 kg (Chelyabinsk, Stony, Russia, 2013)
      
      
* **Cross-Visual Interactivity:** The dashboard uses "Filter" interactions, allowing users to click the Map or Legend to instantly update the Bar Chart and KPI metrics.
* **Dynamic Slicers:** Fully interactive filters for **Year Range**, **Meteorite Name**, and a custom **"Clear All Slicers"** reset button.

## 🛠️ Tech Stack & Skills
* **Visualization Tool:** Power BI Desktop
* **Dataset:** [NASA Open Data Portal - Meteorite Landings](https://data.nasa.gov/Space-Science/Meteorite-Landings/gh4g-9sfh)
* **Data Transformation:** Power Query (M) for ETL processes.
* **Calculations:** DAX (Data Analysis Expressions) for dynamic mass conversion and measures.

## 🧹 Data Cleaning & ETL Process
Before visualization, the raw dataset underwent a rigorous cleaning process in Power Query:
1. **Coordinate Handling:** Filtered out entries with $0,0$ latitude/longitude to ensure map accuracy.
2. **Date Standardizing:** Extracted and cleaned the 'Year' column from timestamps (860 AD – 2013).
3. **Unit Conversion:** Converted mass from grams ($g$) to kilograms ($kg$) using DAX to improve readability for large-scale impacts.
4. **Categorization:** Created a custom column `Meteorite type` to group complex `recclass` values into four simplified categories.
5. **Geospatial Formatting:** Standardized latitude (`reclat`) and longitude (`reclong`) to ensure precise mapping.

## 📂 Repository Structure
* `data/`: Contains the raw and cleaned NASA Meteorite Landings CSV.
* `report/`: The `.pbix` file (Power BI Dashboard).
* `screenshots/`: Images and GIFs of the dashboard in action.
* `README.md`: Project documentation.

## 🚀 How to View the Dashboard
1. Download the `NASA_Meteorite_Analysis.pbix` file from the `report/` folder.
2. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Free).
3. Open the file to interact with the live charts.

---
**Created by Mohammed Saif Shaikh** *Final Year B.Tech Student in AI & Data Science*

Any Questions? Feel free to contact me at ms.sk.3609@gmail.com
