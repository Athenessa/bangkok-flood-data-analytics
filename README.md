# Bangkok Flood Data Analytics 🌧️

**Environmental Data Analysis and Insights**  
A group project for **2107540 Data Science for Environment and Sustainability**.

This project investigates flooding in Bangkok, Thailand, using environmental data analysis, exploratory data analysis (EDA), data visualization, and an optional machine-learning extension. It examines the spatial and temporal distribution of recorded flood events and explores how flood characteristics can support better understanding and management of urban flood risk.

---

## 1. Environmental Problem

Urban flooding is a recurring environmental challenge in Bangkok. It can disrupt transportation and daily activities, damage property, and create risks for public health and safety.

This project uses recorded flood-event data to investigate:

- When flooding events occur and how their frequency varies over time.
- Which Bangkok districts are frequently affected.
- How flood characteristics, including depth and duration, vary across locations and time.
- How data analysis can help communicate flood patterns and inform flood-management decisions.

## 2. Dataset and Sources

The project dataset covers **Bangkok, Thailand, during 2024–2025**. The repository currently documents **841 flood-event records across 43 districts**, stored in Excel format.

The cleaned dataset used for analysis is available in [data/](./data/).

## 3. Data Cleaning and Transformation

The data preparation stage organizes the raw observations into a format suitable for analysis. The cleaned dataset is stored in the data folder.

The machine-learning workflow also documents a specific missing-value decision: **seven district records have missing average flood duration because no flood events were recorded during the observation period**. These values were retained as missing rather than filled with zero, since an average duration is undefined when there are no recorded events. All seven districts were retained for further analysis.

**Details:** [Data and cleaning files](./data/)

## 4. Exploratory Data Analysis (EDA)

EDA is used to understand the dataset before drawing conclusions. The analysis explores the distribution of flood events across time and districts, as well as the characteristics of recorded events.

**Details and supporting files:** [Exploratory Data Analysis folder](./EDA/)

## 5. Data Analysis and Insights Extraction

The current analysis reports the following findings:

- Flood events in the dataset were concentrated in particular months, especially **May, September, and October**.
- **May** recorded the highest number of flooding events.
- **September** exhibited the highest mean flooding duration, indicating that the month with the most events is not necessarily the month with the most persistent flooding.
- Approximately **81.5%** of recorded events occurred during the rainy season.
- Differences in observation coverage between 2024 and 2025 limit direct year-to-year comparisons.

These findings describe the records available in this dataset and should be interpreted in light of the observation-coverage limitation.

**Details and analysis notebook:** [Data Analysis and Insights](./Analysis/)

## 6. Data Visualization

Visualizations communicate the spatial and temporal patterns observed in the data and help make the findings easier to interpret.

**Figures and visualization work:** [Visualization folder](./visualization/)  
**Dashboard work:** [Dashboard folder](./dashboard/)

## 7. Basic Machine Learning (Optional Extension)

The repository includes a machine-learning and budget-allocation extension. Its guiding question is:

> Given a fixed budget, how should Bangkok allocate its flood-management budget across districts to reduce flood risk?

The documented workflow is organized into two stages:

**Stage A — Machine Learning**
1. Combine district budget data and flood observations.
2. Engineer district-level flood-characteristic features.
3. Scale features using StandardScaler.
4. Apply K-Means clustering to group districts with similar flood characteristics.
5. Evaluate and interpret clusters using the elbow method, silhouette score, and cluster profiles.

**Stage B — Budget Optimization**
1. Use district risk profiles and existing budget data.
2. Define budget constraints and intervention scenarios.
3. Develop an optimization model to allocate a fixed budget under explicit assumptions.
4. Compare current and proposed allocations.

The ML folder also references the [UK Government guide to Multi-Criteria Decision Analysis (MCDA)](https://analysisfunction.civilservice.gov.uk/policy-store/an-introductory-guide-to-mcda/).

**Details and notebook:** [Machine Learning folder](./ML/)

## 8. Environmental Interpretation

The findings distinguish between flood **frequency** and flood **persistence**: May had the most recorded events, while September had the longest mean duration. This distinction is relevant when interpreting flood impacts and considering district-level management priorities.

The rainy-season concentration (approximately 81.5% of records) provides temporal context for the observed events. However, differences in data coverage between 2024 and 2025 mean that direct comparisons across those years require caution.

The optional ML extension explores how districts with similar flood characteristics might be grouped and how those profiles could inform transparent, constraint-based budget scenarios. Any proposed allocation should be interpreted in light of the model assumptions and available data.

## 9. Repository Guide

Use the links below to open the detailed work for each project component.

| Project component | Folder / contents |
|---|---|
| Dataset and data preparation | [data/](./data/) |
| Exploratory Data Analysis (EDA) | [EDA/](./EDA/) |
| Data analysis and insights extraction | [Analysis/](./Analysis/) |
| Data visualization | [visualization/](./visualization/) |
| Interactive dashboard | [dashboard/](./dashboard/) |
| Basic machine learning and budget optimization | [ML/](./ML/) |
| Reports and written findings | [reports/](./reports/) |
| Additional notebooks | [notebook/](./notebook/) |

Main analysis notebook: [Analysis/Part4_Data_Analysis_and_Insights.ipynb](./Analysis/Part4_Data_Analysis_and_Insights.ipynb)  
Visualization notebook: [visualization/data_group.ipynb](./visualization/data_group.ipynb)  
Machine-learning notebook: [ML/ML.ipynb](./ML/ML.ipynb)

## 10. Tools and Technologies

The project README currently identifies the following tools and libraries:

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Plotly
- Scikit-learn
- Streamlit

## 11. Project Deliverables

For Project 1, the assignment requires a GitHub repository and a group presentation. The presentation should communicate the complete analytical workflow, from data collection through findings and conclusions.

- **Course:** 2107540 Data Science for Environment and Sustainability
- **Project:** Project 1 — Group Project (20%)
- **Presentation:** 18 November 2026
- **Presentation duration:** 10 minutes per group
- **Repository deliverable:** Project documentation, data, analysis, and supporting materials

## 12. Project Team

- **Idea** (Kanrutairat D.)
- **Gin** (Jidapa J.)
- **Ying** (Chalermkwan P.)

---

## Project Status

The repository contains the cleaned dataset, EDA materials, analysis notebook, visualizations, dashboard materials, and an optional machine-learning workflow. Key findings are summarized above; supporting details are linked in the [Repository Guide](#9-repository-guide).
