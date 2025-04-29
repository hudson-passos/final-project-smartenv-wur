# 🇵🇱 Investigating Causes and Impacts of Air Pollution in Poland

## 📘 Background

The learning goals were defined to align both with data science skills I wanted to develop and with the technical needs of the group project. Given that the course lasted only three weeks, we aimed for goals that were realistic yet meaningful. The individual learning plan can be found [here](https://github.com/hudson-passos/DSSE-Individual-Portfolio/blob/main/01.%20Introduction.ipynb).

Our group selected **air quality in Europe** as the main theme, ultimately focusing on **Poland** due to the high levels of air pollution and abundance of accessible data. The project was titled:

> **Investigating Causes and Impacts of Air Pollution in Poland**

We defined three objectives:

1. **Analyze the contribution of sources of Nitrogen Oxides (NOx) to air pollution in Poland in 2019**  
2. **Investigate the relationship between traffic and emissions using machine learning and predict emissions in 2023**  
3. **Investigate the relationship between the annual average concentration of PM2.5 and the rate of death caused by respiratory diseases**

Task responsibilities were distributed among group members:

- Objective 1: **Qin Xu (Olive)** and **Hudson Passos**
- Objective 2: **Dong Liang**
- Objective 3: **Pamungkas Intam** and **Sabrina Ramadwiriani**

## 🎯 Learning Goals

The first objective aligned closely with my individual learning goals:

1. **Geospatial analysis using GeoPandas**  
   We used GeoPandas extensively for spatial operations and mapping. While subplots and object handling posed some challenges, its similarity to Pandas made the learning curve manageable. I was able to replicate most GIS operations directly in Python.

2. **Combining data from multiple sources**  
   We merged diverse datasets into integrated dataframes. While this was time-consuming, it helped improve my data cleaning and merging skills. I still aim to improve the use of reusable functions and class-based code.

3. **GitHub for code sharing**  
   We used GitHub as our main code-sharing platform. Although we didn't fully utilize features like version control, it was a valuable introduction to collaborative coding. The project repository is available [here](https://github.com/hudson-passos/DSSE).

---

## 📂 Data Sources

| Theme        | Source                                 | Description                                       | Type     | Link |
|--------------|----------------------------------------|---------------------------------------------------|----------|------|
| Boundaries   | GIS.Box                                | Poland admin boundaries (provinces, counties)     | Shapefile | [Link](https://gis-support.pl/baza-wiedzy-2/dane-do-pobrania/granice-administracyjne/) |
| Air Pollution| Inspekcja Ochrony Środowiska           | NOx emissions (kg), point-based measurements       | CSV      | [Link](https://powietrze.gios.gov.pl/pjp/archives) |
| Traffic      | Statistics Poland                      | NOx emissions from transport (tonnes), by province | CSV      | [Link](https://transtat.stat.gov.pl/) |
| Industry     | European Environment Agency            | Industrial NOx emissions (kg), point-based         | CSV      | [Link](https://www.eea.europa.eu/en/datahub/datahubitem-view/9405f714-8015-4b5b-a63c-280b82861b3d) |

A full spreadsheet of dataset descriptions is available [here](https://github.com/hudson-passos/DSSE/raw/main/Report%20and%20Presentation/Data%20Availability.xlsx).

---

## 🧪 Methodology

The methodology involved extracting pollution-related information and associating it with administrative boundaries to assess contributions to air pollution. Key steps:

- Download and inspect datasets
- Clean and filter relevant data (e.g., NOx emissions in Poland)
- Merge multiple datasets into a single, integrated dataframe
- Visualize data using maps and bar charts
- Prepare the data for machine learning:
  - Standardize variables  
  - Train/test split  
  - Grid search for hyperparameters  
  - Train **XGBoost** model  
  - Evaluate using cross-validation  
  - Analyze **feature importance**

---

## 💻 Implementation

The full implementation for Objective 1 is available [here](https://github.com/hudson-passos/DSSE-Individual-Portfolio/blob/main/Objective%201_Analyze_the_contribution_of_sources_of_Nitrogen_Oxides_(NOx)_to_the_air_pollution_in_Poland_in_2019.ipynb).

---

## 📊 Results

- The **energy sector** emerged as the primary NOx emission source, especially in Slaskie, Lodzkie, and Mazowieckie provinces.
- **Motor vehicle traffic** was the second-largest contributor, most prominent in Mazowieckie (Warsaw).
- The **mining industry** had a moderate but geographically widespread impact.
- **Intensive livestock** showed negligible NOx emissions, mostly contributing **NH₃**, **CH₄**, **N₂O**, and **PM10** instead.

In the **feature importance analysis**, the results differed:

- **Energy sector** emissions were still the top predictor (score: 32)
- **Chemical industry** ranked second (score: 20), due to inverse correlation patterns
- **Mineral industry** came third (score: 10)

This difference highlights that **feature importance reflects correlation, not causal contribution**.

---

## ✅ Conclusions on Results

- **Direct data analysis** using graphs and maps was the most reliable method for identifying key pollution sources.
- **Feature importance** was less suitable for causal understanding, as it may highlight correlated but less directly impactful variables.
- This distinction became clear when the chemical industry, a minor emitter, showed high predictive importance due to spatial inverse correlation.

---

## 🎯 Reflections on Learning Goals

All learning goals were successfully met:

- I became confident in using **GeoPandas** for spatial analysis.
- I learned to integrate and clean **multisource datasets**.
- I developed basic proficiency in **GitHub** for collaboration and versioning.

This experience showed the value of working on topics of personal interest and has strengthened my skills for future projects and research.

---
