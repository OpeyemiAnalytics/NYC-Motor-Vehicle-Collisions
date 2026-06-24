# NYC-Motor-Vehicle-Collisions
Power BI dashboard analyzing 238,421 NYC motor vehicle collision records (2021-2023) to identify accident patterns by time, location and contributing factors.
# 🚨 Impact Zone: NYC Motor Vehicle Collision Analysis

## Project Overview
Analysis of 238,421 motor vehicle collisions reported by the 
New York City Police Department covering 2021-2023. 
Each record represents an individual collision including date, 
time, location, vehicles involved, victims and contributing factors.
This analysis identifies accident patterns by time, location 
and contributing factors to support data-driven road safety decisions.

## Dataset
- Source: Digitaleydrive Data Analytics Bootcamp
- Size: 238,421 collision records
- Period: 2021-2023
- Columns: 18 fields

## Tools Used
- Power BI Desktop - Visualization & Dashboard
- Power Query - Data Cleaning & Transformation
- DAX - Calculated Measures

## Data Cleaning Steps
- Checked for duplicate records
- Replaced null Contributing Factor Vehicle 1 → "Unspecified"
- Replaced null Persons Injured → 0
- Replaced null Borough → "Not Recorded"
- Replaced null Street Name → "Not Recorded"
- Left Latitude, Longitude & Cross Street nulls as blank
  (location data cannot be imputed without introducing false information)
- Extracted Month Name, Month Number from Crash Date
- Extracted Day Name, Day Number from Crash Date
- Extracted Hour from Crash Time
- Created Month Name column (Jan-Dec) for cleaner visuals
- Created Day Name column (Sun-Sat) for cleaner visuals
- Sorted months chronologically using Month Number
- Sorted days Sun-Sat using Day Number
- Created manual Victim Breakdown reference table containing 
  aggregated Injured and Killed figures for Motorists, 
  Pedestrians and Cyclists
- Created % of Total Collisions measure for monthly analysis

## Key Findings

### Question 1 - Monthly Patterns
- Collisions ranged from 17K to 25K per month
- March recorded highest collisions (25K)
- December recorded lowest (17K)
- % of total accessible via tooltip on monthly chart
- Winter months consistently showed higher collision rates
  than summer months

### Question 2 - Day & Hour Patterns
- Fridays most dangerous day (37K collisions)
- Sundays safest day (31K collisions)
- Peak collision hour: 4PM (Hour 16) with 15,100 collisions
- Safest time to drive: 4AM with only 4,300 collisions
- Clear evening rush hour pattern visible in hourly trend

### Question 3 -  Most Dangerous Street
- Belt Parkway recorded highest collisions at 3,700
- Representing approximately 1.6% of all reported collisions
- Broadway second most dangerous at 2,800 collisions
- Atlantic Avenue, Long Island Expressway and Brooklyn 
  Queens Expressway tied at 2,200 each

### Question 4 - Contributing Factors
- Unspecified causes: 60K (25%) — cause unknown
- Driver Inattention/Distraction: 58,308 (24.5%)
- Failure to Yield: 17K
- Following Too Closely: 16K
- Over 50% of collisions lack clear preventable attribution

**Fatal Accidents Specifically (613 fatal accidents):**
- Driver Inattention/Distraction remained leading cause
- Failure to Yield and Unsafe Speed disproportionately 
  higher in fatal vs non-fatal accidents
- Speed and right-of-way violations carry significantly 
  higher death risk
- Pedestrians faced highest fatality rate at 1.5% vs 
  motorists at 0.3%
  
## Bonus Insight - Victim Analysis
- Motorists most injured (81,428) but lowest fatality rate (0.3%)
- Pedestrians fewer injuries (18,877) but highest fatality 
  rate (1.5%) — 5x more likely to die than motorists
- Cyclists least involved (10,932 injured, 47 killed)
- Urgent need for dedicated pedestrian safety infrastructure 
  in high collision boroughs

  ## Recommendations
1. Launch distracted driving enforcement campaign -
   targeting phone use during peak Friday 4PM hours
2. Prioritize pedestrian safety infrastructure on 
   Belt Parkway and Broadway
3. Increase traffic monitoring during winter months 
   when collision rates peak
4. Deploy additional traffic officers during 
   Friday evening rush hour (3PM-6PM)
5. Investigate the 25% unspecified causes -
   better incident reporting systems needed

## Dashboard Preview
[<img width="1524" height="857" alt="image" src="https://github.com/user-attachments/assets/c548cf9f-7b00-4d57-9ddb-c0b505522a17" />]


## Author
**Opeyemi Taiwo** | Business Intelligence & Financial Analyst
[LinkedIn](www.linkedin.com/in/opeyemi-taiwo-565985185)
