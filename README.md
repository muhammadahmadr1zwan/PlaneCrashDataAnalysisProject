# **Analyzing Trends and Insights in Global Commercial Airplane Crashes**

## **Introduction**
This project aims to analyze global commercial airplane crashes to uncover critical insights about their frequency, causes, and impact. By utilizing statistical methods and data visualization, this project identifies trends, explores contributing factors, and highlights patterns in crash occurrences and fatalities.

### **Objective**
- Examine the frequency and causes of airplane crashes.
- Analyze the relationship between crash fatalities, causes, and economic factors such as GDP per capita.
- Visualize key metrics to provide insights into the data.

---

## **Dataset**
- **Source:** `commercialairplanecrashes.csv`
- **Key Features:**
  - **Numerical:** `Fatalities`, `Country GDP per Capita`
  - **Categorical:** `Cause of Crash`, `Year`, `Country`

### **Sample Dataset Overview**
| **Feature**                | **Description**                                   |
|-----------------------------|---------------------------------------------------|
| `Cause of Crash`            | Cause of the crash (e.g., mechanical error).      |
| `Fatalities`                | Total number of fatalities in the crash.          |
| `Country`                   | Country where the crash occurred.                 |
| `Year`                      | Year of the crash.                                |
| `Country GDP per Capita`    | GDP per capita of the country where the crash occurred. |

---

## **Exploratory Data Analysis**
### **Steps Undertaken:**
1. **Crash Cause Analysis:**
   - Frequency distribution of crash causes.
   - Visualized the most common causes using bar plots.

2. **Fatalities Analysis:**
   - Analyzed fatalities by year.
   - Mapped crash locations to identify regional trends.

3. **Economic Correlation:**
   - Investigated the relationship between GDP per capita and crash occurrences.
   - Observed that most crashes occur in countries with GDP per capita below specific thresholds:
     - **82.7%** of crashes: GDP < $20,000.
     - **62%** of crashes: GDP < $10,000.
     - **51.7%** of crashes: GDP < $5,000.

### **Challenges in Data Preparation:**
1. **Handling Missing or Ambiguous Data:**
   - Ensured all columns had complete and valid data.

2. **Standardizing Categorical Data:**
   - Encoded categories (e.g., causes, countries) for machine learning compatibility.

3. **Outlier Detection:**
   - Identified and flagged extreme values in fatalities using statistical methods.

---

## **Visualization Highlights**
1. **Bar Plot: Crash Causes**
   - Displays the frequency of each crash cause.
   - Highlights the most common contributing factors to crashes:
     
     ![image](https://github.com/user-attachments/assets/86150bf2-6a5b-4a62-8645-44b3b2e26bc3)


2. **Fatalities Over Time**
   - Displays fatalities (x-axis) for each year (y-axis), with labeled axes highlighting fatalities per year for easy interpretation:
     
      ![image](https://github.com/user-attachments/assets/227c2d74-bc79-43f8-aa3a-e2958cfd50b5)
   - Displays total fatalities (x-axis) by year (y-axis), with each dot representing yearly fatalities, highlighting trends over time:
     
      ![image](https://github.com/user-attachments/assets/9efc1253-c8d6-4127-b1a9-46c257872c95)

     
3. **Economic Analysis:**
   - Bar plot comparing GDP per capita of countries to crash occurrences:
     
     ![image](https://github.com/user-attachments/assets/65e8270f-afe4-4eca-8451-a0fcef6ca1e0)



4. **Scatter Plot: Fatalities vs. Causes**
   - Displays crash causes (y-axis) against fatalities (x-axis), highlighting fatalities for each cause with labeled axes for easy interpretation:
     
      ![image](https://github.com/user-attachments/assets/24892faa-c222-48a2-9e6c-e39dbb23182a)


---

## **Methodology**
### **Data Preprocessing**
1. **Categorical Encoding:**
   - Converted crash causes and countries into numerical representations using one-hot encoding.

2. **Outlier Detection and Handling:**
   - Data points with extreme fatality values were removed using the interquartile range (IQR) method.

3. **Data Normalization:**
   - Standardized numerical columns (e.g., GDP, fatalities) for consistent analysis.

### **Data Analysis Tools:**
- **Python Libraries:**
  - `R` for data manipulation, visualization, and numerical operations
---

## **Results**
### **Key Insights:**
1. **Crash Causes:**
   - Mechanical errors, weather conditions, and pilot error are among the most frequent causes.
   - Weather-related crashes tend to result in higher fatalities.

2. **Fatalities and Economic Factors:**
   - Lower GDP per capita correlates with higher crash frequencies, indicating potential links to infrastructure and safety regulations.

3. **Yearly Trends:**
   - Annual fatalities fluctuate, with peaks observed in specific years tied to catastrophic events.

### **Best Visualization:**
The bar plot correlating GDP per capita with crash frequency effectively illustrates the economic disparities influencing aviation safety.

---

## **Conclusion**
### **Summary:**
This project highlights the critical factors influencing global airplane crashes, emphasizing economic disparities and common causes. The findings can inform future safety measures and resource allocation to reduce crash frequencies and fatalities.

