# 🚦 Road Accident Dashboard (Excel)

## 📌 Project Overview

This project presents an interactive **Excel dashboard** that analyzes road accident data to uncover trends related to accident severity, road conditions, lighting, and locations.  
The dashboard helps transform raw accident data into clear, actionable insights.

---

## 🎯 Objectives

- Analyze accident severity distribution (Fatal, Serious, Slight)
- Identify accident trends over time
- Understand the impact of road type, road surface, and lighting conditions
- Provide an interactive tool for data-driven insights

---

## 📊 Dashboard Features

- **KPIs**
  - Total Accidents
  - Total Fatal Injuries
  - Total Serious Injuries
  - Total Slight Injuries
- **Visual Analysis**
  - Accident count by month
  - Accident distribution by road type
  - Accident frequency by road surface
  - Accident distribution by lighting & visibility
  - Accident count by local authority district
- **Interactive slicers**
  - Year
  - Accident severity
  - Weather conditions
  - Road type

---

## 🧮 Measures Used (DAX)

```text
Total Accidents = COUNT(Accident_Index)

Fatal injuries =
CALCULATE(
    COUNT(Accident_Index),
    Table1[Accident_Severity] = "Fatal"
)

Serious injuries =
CALCULATE(
    COUNT(Accident_Index),
    Table1[Accident_Severity] = "Serious"
)

Slight injuries =
CALCULATE(
    COUNT(Accident_Index),
    Table1[Accident_Severity] = "Slight"
)

Total number of casualties = SUM(Number_of_Casualties)

Total number of vehicles involved = SUM(Number_of_Vehicles)


```

📈 Dashboard Charts Explanation
1️⃣ Accident Count by Month

Why this chart was created:
To identify seasonal and monthly trends in road accidents.

What it shows:
This line chart highlights how accident frequency changes across months, helping detect peak accident periods.

Insight:
Certain months show higher accident counts, which may be linked to weather conditions, holidays, or traffic volume increases.

2️⃣ Accident Distribution by Road Type

Why this chart was created:
To understand which road types are most associated with accidents.

What it shows:
A bar chart comparing accident counts across road types such as single carriageway, dual carriageway, roundabout, and slip roads.

Insight:
Single carriageways have the highest number of accidents, indicating higher risk compared to other road types.

3️⃣ Accident Severity Distribution

Why this chart was created:
To analyze how severe road accidents are overall.

What it shows:
A donut chart displaying the proportion of accidents classified as Slight, Serious, or Fatal.

Insight:
The majority of accidents result in slight injuries, while fatal accidents represent a small but critical percentage that requires attention.

4️⃣ Accident Distribution by Lighting & Visibility

Why this chart was created:
To evaluate how lighting conditions affect accident occurrence.

What it shows:
A pie chart comparing accidents during daylight, darkness with street lighting, and darkness without lighting.

Insight:
Most accidents occur during daylight, mainly because traffic volume is highest at that time, while poor lighting still contributes to increased risk.

5️⃣ Accident Frequency by Road Surface

Why this chart was created:
To analyze the impact of road surface conditions on accident frequency.

What it shows:
A bar chart comparing accidents on dry, wet/damp, icy, snowy, and flooded road surfaces.

Insight:
Wet or damp road surfaces significantly increase accident frequency compared to dry roads.

6️⃣ Accident Count by Local Authority District

Why this chart was created:
To identify geographic areas with higher accident concentrations.

What it shows:
A bar chart ranking local authority districts by accident count.

Insight:
Some districts consistently show higher accident rates, which can help authorities focus safety measures and traffic control efforts.

7️⃣ KPI Cards (Top Metrics)

Why these KPIs were created:
To give an immediate high-level summary of road safety performance.

KPIs Included:

Total Accidents

Fatal Injuries

Serious Injuries

Slight Injuries

Insight:
These KPIs allow quick comparison across filters (year, weather, road type) and support fast decision-making.
