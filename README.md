# Trend-Analysis-of-Aerosol-Optical-Depth-in-Indian-Cities

## **Project Overview**
This project focuses on analyzing the long-term trends of **Aerosol Optical Depth (AOD)** over India using **MODIS MCD19A2** satellite data from **2001 to 2023**. The goal is to assess atmospheric aerosol variations and their impact on air quality and climate change. The analysis utilizes statistical techniques like **Mann-Kendall trend detection** and **Sen’s Slope estimation** to determine significant changes in AOD levels over time.

## **Objective**
- Analyze AOD trends across India from 2001 to 2023.
- Identify increasing or decreasing trends in AOD values using statistical methods.
- Extract AOD data for **20 major Indian cities** for city-wise trend evaluation.
- Handle large geospatial datasets efficiently with memory constraints.
- Visualize trends to support environmental monitoring and policymaking.

## **Dataset**
- **Source:** MODIS MCD19A2 (MAIAC Land Aerosol Optical Depth)
- **Format:** `.tif` files organized by year and month
- **Spatial Coverage:** India
- **Temporal Coverage:** 2001–2023
- **Resolution:** 1 km

## **Methods & Tools Used**
### **Data Acquisition & Processing**
- Downloaded MODIS AOD data via **Google Earth Engine (GEE)**.
- Processed `.tif` images using **Python (rasterio, numpy, pandas)**.
- Structured and sorted monthly data for chronological consistency.

### **Trend Analysis**
- **Mann-Kendall test** for detecting statistically significant trends.
- **Sen’s Slope estimator** to calculate the rate of AOD change over time.
- Handled **missing values (NaN)** without affecting trend estimation.

### **Visualization & Interpretation**
- Plotted **time-series AOD trends** using `matplotlib` and `seaborn`.
- X-axis represents years (2001–2023) to show long-term changes.

## **Project Workflow**
1. **Data Download:** Fetch monthly MODIS AOD `.tif` images from GEE.
2. **Preprocessing:** Organize, clean, and structure data for analysis.
3. **Trend Detection:** Apply Mann-Kendall and Sen’s Slope analysis.
4. **City-Wise Analysis:** Extract AOD for **20 major Indian cities**.
5. **Visualization:** Generate plots to illustrate trends over time.

## **Results & Impact**
- Identified an **increasing AOD trend**, indicating worsening air pollution in urban regions.
- Developed an optimized Python workflow for **satellite data analysis**.
- The findings provide insights into **air quality trends** for policymakers and researchers.

## **Dependencies & Requirements**
To run this project, install the following Python libraries:
```bash
pip install numpy pandas rasterio matplotlib seaborn scipy
```

## **Usage**
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/AOD-Analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd AOD-Analysis
   ```
3. Run the main script for trend analysis:
   ```bash
   python analyze_aod.py
   ```

## **Future Enhancements**
- Extend analysis to include other environmental factors (e.g., temperature, precipitation).
- Automate data extraction and processing using **Google Earth Engine API**.
- Improve visualization with interactive dashboards (e.g., using Plotly or Dash).

## **Contributors**
- **Shristi Pandey** – Data Analysis & Implementation
- **Mentor:** Dr. Manoj Kumar Mishra (ISRO)

## **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
