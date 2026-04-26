# Sleep Pattern & Lifestyle Analysis: A Human Performance Case Study
## An End-to-End Data Analytics Project investigating the drivers of daily fatigue.

## Overview
This project investigates the "Sleep Satisfaction Gap"—why a majority of individuals feel fatigued despite meeting average sleep duration milestones. By analyzing a dataset of 103 survey respondents, this study identifies how morning nutrition and nighttime digital habits influence perceived tiredness more than sleep quantity alone.

## Problem Statement
Most health advice focuses exclusively on "sleep hours" (Quantity). However, productivity remains low even for those meeting these goals.
    
   **The Goal:** Identify if "Quality" factors (Breakfast, Phone Habits) provide a higher Return on Investment (ROI) for daily alertness than simply increasing sleep time.
   
## Dataset
- Source: sleep_data.csv (Kaggle)
- Records: Survey based lifestyle and sleep data

## Dashboard Preview
![Sleep Pattern & Lifestyle Analysis Dashboard](sleep_dashboard.png)

## Business Intelligence Dashboard
The final dashboard was built in Excel, featuring dynamic KPIs, Slicers for interactivity, and a high-contrast "Dark Mode" aesthetic for professional readability.

# Key Performance Indicators (KPIs)
- **Average Sleep Duration:** 6.7 hours
- **Average Tiredness Level:** 3.1 / 5
- **Sleep Dissatisfaction Rate:** 66% of respondents feel they do not get enough sleep.

## The Analytical Workflow (Data Preparation)
To ensure the integrity of the insights, I followed a professional data pipeline:
   - **Data Normalization:** Cleaned and standardized Binary Variables (Breakfast, Phone Usage, Phone Reach) to ensure 100% accuracy in Pivot Table aggregations.
   - **Feature Engineering (Data Binning):** Created three distinct sleep cohorts to reduce granularity noise:
     * High Risk (≤5 hrs)
       
     * Sub-optimal (6–7 hrs)
       
     * Target/Healthy (≥8 hrs)
       
   - **Quantitative Scaling:** Analyzed the Tired_Level as a 1–5 Likert Scale, calculating weighted averages to provide a "Fatigue Score" for different lifestyle segments.
     
      * **1 - Peak Vitality** (Maximum energy; optimal cognitive performance)
     
      * **2 - Functional** (Normal daily energy; no significant fatigue reported)
     
      * **3 - Moderately Fatigued**(Population Mean: 3.1) Notable dip in energy; productivity starts to decline
     
      * **4 - Highly Exhausted** (Significant fatigue impacting productivity and mood)
     
      * **5 - Critical Fatigue** (Extreme exhaustion, difficulty performing tasks effectively)
     
   - **Statistical Validation (Correlation Analysis):** Executed a Pearson Correlation in excel, resulting in r = -0.19. This mathematically confirmed a weak relationship between sleep hours and fatigue, identifying that "Quantity" alone was not the primary driver of tiredness.
   - **Integrity Check:** Resolved data type inconsistencies (Text vs. Number) to ensure all KPI cards reflected accurate mathematical means.
   - **Pivot Table Architecture:** Developed a robust backend using Pivot Tables to allow for multi-dimensional filtering via Slicers.
   - **Visualization Strategy:**
     * **Donut Charts:-** Used to represent the distribution of the binary variable “Enough Sleep”.
     
     * **Bar Charts:-** Used for categorical comparisons such as Breakfast habits and Phone Usage.
     
     * **Scatter Plots:-** Used to visualize the correlation between Sleep Hours and Tiredness Averages, identifying non-linear trends across different sleep cohorts.

## Key Insights
   - **The Sleep Satisfaction Gap:** While the average sleep duration is 6.7 hours, there is a 66% dissatisfaction rate regarding sleep quality. This highlights a significant gap between time spent in bed and actual recovery.
   - **The Nutritional Lever:** Analysis identifies morning nutrition as a high-impact, low-cost intervention. Consistent breakfast consumption is associated with a 15% reduction in fatigue levels (2.9 vs. 3.4 baseline), proving more effective for alertness than sleep duration alone.
   - **The Digital Masking Paradox:** The data reveals a surprising trend: individuals who reported No late-night phone usage actually had a higher fatigue score (3.2) than those who did (3.1). This suggests a 'Digital Stimulation' effect where screen time might be temporarily masking perceived tiredness, even if it's not providing real rest.
     
## Business Takeaways:
- **The "Breakfast Boost":** For those getting 8+ hours of sleep, skipping breakfast led to a tiredness spike of 3.7. Eating breakfast is the fastest way to stabilize energy, regardless of sleep duration.
- **Fix the "6-7 Hour" Trap:** This group represents the most common sleep bracket but lacks a strong "recovery" score. For these individuals, habit changes (like removing the phone) saw tiredness drop from 3.1 to 2.3.
- **The 5-Hour Danger Zone:** Once sleep drops below 5 hours, fatigue reaches critical levels (up to 4.4). At this threshold, lifestyle habits struggle to compensate for the physiological lack of rest.

## Project Limitations
To maintain transparency, the following limitations were considered:
- **Sample Size (N = 103):** The dataset is relatively small, so findings are useful for trends but may not represent the entire population.
- **Self-Reporting Bias:** Tiredness levels are based on personal perception, which can vary between individuals.
- **Correlation vs Causation:** The analysis identifies relationships (e.g., breakfast and tiredness) but does not prove direct cause-and-effect.
  
## Conclusion
This study proves that sleep quantity is not the only factor in energy. While 6.7 hours is the average sleep time, 66% of people still feel tired. The data shows a weak correlation (r = -0.19) between sleep hours and tiredness, meaning that lifestyle choices—like eating breakfast and putting the phone away—are often more important than the time spent in bed. To truly beat fatigue, we must focus on quality habits, not just the clock.
