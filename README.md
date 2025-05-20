# powerbi-climate-change: Causes and Its Effects

In this project, I explore the major causes and effects of global climate change. Using data analysis and interactive visualizations, I highlight the top contributing countries and industries responsible for emissions like CO₂ and CH₄.

I also examine the rise in natural disasters linked to climate change, focusing on the most destructive events and their cascading impacts. Key insights include alarming figures on climate-related deaths, soil erosion due to increased precipitation, and declining agricultural output.

This project is intended to raise awareness and urge action — especially from high-GDP and high-population nations — toward meaningful climate solutions.

---

## 🗂️ Data Sources & Model

This project uses 4 different publicly available datasets from trusted global sources:

- **Climate Data**: Temperature & precipitation trends from the [World Bank](https://www.kaggle.com/theworldbank/world-bank-climate-change)
- **Natural Disasters**: Disaster impact data from [EM-DAT](https://public.emdat.be/)
- **Emissions**: CO₂ and GHG emissions by country/sector from the [World Resources Institute](https://www.wri.org/data/climate-watch-cait-country-greenhouse-gas-emissions-data)
- **Country Info**: GDP, population & region data from the [World Factbook](https://www.kaggle.com/fernandol/countries-of-the-world)

These were modeled in Power BI using a relational schema. The `Countries` table serves as the core dimension, linking climate metrics, emissions, disasters, and socioeconomic data through one-to-many relationships. All datasets were cleaned and integrated to support interactive visual analysis.

---

## 🔍 Analysis & Key Discoveries

### 🌪️ Disasters Caused by Climate Change

A traffic light visual represents disaster severity:

- ✅ **Green**: No major consequences observed.
- 🟡 **Yellow**: Subtypes led to limited associated disasters.
- 🔴 **Red**: Subtypes caused severe associated disasters.

**Trends Over Time**:

- **1960–1990**: Mostly green (low severity).
- **Post-1990**: Increase in red severity (rising impact).

![image](https://github.com/user-attachments/assets/efb5423f-0df4-4c06-b514-b25ef8d94beb)
- Shows data from 1960-1970s, where the number of low severity disasters were more than high severity


---

### 🌍 Global Emissions

From 1990 to 2011, the following GHG emissions were recorded:

- **Methane (CH₄)**: 307.51K MtCO₂e
- **Nitrous Oxide (N₂O)**: 161.85K MtCO₂e
- **F-Gases**: 22.69K MtCO₂e

![image](https://github.com/user-attachments/assets/cec4eb30-a74d-4302-9c20-9b43a504220c)

Methane contributed the most. Bookmarks in Power BI allow toggling between graphs and numeric views.

---

### 🌱 Soil Erosion Analysis

#### 1) Filled Map

- **1990–1992**: Minimal erosion in developed countries.
  ![image](https://github.com/user-attachments/assets/8bcd93cf-26cd-4c0b-9956-e8a06defe470)
  
- **1998–2003**: Erosion rises in Africa and Asia due to industrial and agricultural growth.
 - ![image](https://github.com/user-attachments/assets/7baa28e6-4c0b-45ff-b813-237b30b2b3af)

- **2008–2011**: Intensified erosion in lower-income regions.
 - ![image](https://github.com/user-attachments/assets/a2655b0a-0137-4b25-a5ff-72d867f8554a)

#### 2) Erosion vs. Precipitation (Area Chart)

![image](https://github.com/user-attachments/assets/aeb799dc-66fe-4b93-a57d-9634cef395d2)


- Soil erosion trends follow precipitation patterns.
- Lower-income countries suffer more due to lack of mitigation infrastructure.

---

## 🌍 Population & Climate Change

Analyzing effects of population density on temperature, precipitation, and agriculture (1971–2011).

### 1️⃣ Climate Risk Index Map

![image](https://github.com/user-attachments/assets/42423ca9-bb9c-460e-aaff-ba432be6c17e)

- Map shows exposure to extreme weather events.
- Higher population density often means greater risk.

### 2️⃣ Population Density vs. Crop Yield

![image](https://github.com/user-attachments/assets/4a8d02cf-7155-45b7-8ca1-623635c55881)

- Lower density countries show higher crop yield.
- Agriculture:
  - **17%** of GHG emissions from activities like deforestation
  - **7–14%** from land-use changes
- CH₄ and N₂O have higher warming potential than CO₂.

### 3️⃣ Rwanda Gauge Chart

![image](https://github.com/user-attachments/assets/f5d7547d-8ef3-4c95-8a14-441dac88a477)

- Gauge compares annual precipitation vs. crop yield in Rwanda.

**Insights**:

- **1961–2016**: Significant rainfall fluctuations
- **Eastern Rwanda**: Frequent dry spells (Sep–Dec)
- **Northern/Western**: Intense, shorter rainy seasons = higher erosion

**Conclusion**: Shorter rainy seasons and dry spells reduce crop output in countries like Rwanda.

---

> 📈 This project showcases the deep connections between human activity, climate change, and environmental outcomes. The Power BI dashboard offers data-driven insights to support global climate awareness and action.
