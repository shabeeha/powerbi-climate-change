# powerbi-climate-change- Causes and its effects
In this project, I explore the major causes and effects of global climate change. Using data analysis and interactive visualizations, I highlight the top contributing countries and industries responsible for emissions like CO₂ and CH₄.

I also examine the rise in natural disasters linked to climate change, focusing on the most destructive events and their cascading impacts. Key insights include alarming figures on climate-related deaths, soil erosion due to increased precipitation, and declining agricultural output.

This project is intended to raise awareness and urge action — especially from high-GDP and high-population nations — toward meaningful climate solutions.


## 🗂️ Data Sources & Model

This project uses 4 different publicly available datasets from trusted global sources to come to the inferences:
- **Climate Data**: Temperature & precipitation trends from the [World Bank](https://www.kaggle.com/theworldbank/world-bank-climate-change)
- **Natural Disasters**: Disaster impact data from [EM-DAT](https://public.emdat.be/)
- **Emissions**: CO₂ and GHG emissions by country/sector from the [World Resources Institute](https://www.wri.org/data/climate-watch-cait-country-greenhouse-gas-emissions-data)
- **Country Info**: GDP, population & region data from the [World Factbook](https://www.kaggle.com/fernandol/countries-of-the-world)

These were modeled in Power BI using a relational schema. The `Countries` table serves as the core dimension, linking climate metrics, emissions, disasters, and socioeconomic data through one-to-many relationships.

All datasets were cleaned and integrated into a relational model to support interactive visual analysis.

## 🔍 Analysis & Key Discoveries

### 🌪️ Disasters Caused by Climate Change
A traffic light visual is used to represent the severity of disasters:
- **Red**: Disaster subtypes caused associated disasters that continued or escalated.
- **Yellow**: Disaster subtypes led to associated disasters but with limited impact.
- **Green**: No major consequences observed.

### 📈 Trends in Natural Disasters
Using filters, we observe:
- **1960–1990**: Most disasters are marked green (low severity).
- **Post-1990**: Increase in red severity, showing a rising trend in destructive events.

![image](https://github.com/user-attachments/assets/d778b483-7c4d-413c-a2d5-04efbfbb255a)
Image shows disasters from 1960- 1970s, which shows more low severity disasters


### 🌍 Global Emissions
From 1990 to 2011:
- **Methane (CH₄)**: 307.51K MtCO₂e
- **Nitrous Oxide (N₂O)**: 161.85K MtCO₂e
- **F-Gases**: 22.69K MtCO₂e  
Methane contributed the most to global greenhouse emissions. Power BI bookmarks allow toggling between gases for comparison.
![image](https://github.com/user-attachments/assets/0e548a2c-0e61-4302-88fa-f7d948a3dac0)


### 🌱 Soil Erosion Analysis
The report explores soil erosion trends over time by country and income group.

#### Key Visualizations:
- **1) Summary Table (Matrix)**:  
  Shows a hierarchy of indicators: Series Code → Name → Definition → Source. Offers a statistical summary to support deeper insights.

- **2) World Map (Filled Map)**:  
  - **1990–1992**: Minimal erosion in developed countries.
  - **1998–2003**: Rising erosion in parts of Africa and Asia.
  - **2008–2011**: Intensified impact in lower-income regions.

- **3) Erosion vs. Precipitation by Income Group (Area Chart)**:  
  Soil erosion closely follows precipitation trends. Lower-income countries face greater erosion, suggesting that advanced techniques in high-income regions help mitigate the impact.

### 🤖 Auto-Generated Insights
Power BI's AI features helped surface key KPI-driven insights directly within the dashboard.


