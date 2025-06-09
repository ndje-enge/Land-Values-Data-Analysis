# French Land Value Data Analysis (2020 & 2024)

This project analyzes land and property values in different areas of France using datasets from [data.gouv.fr](https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres/).

You can download the land and property values datasets on the previous link. 

## Project Overview

The analysis focuses on comparing the real estate market between 2020 (an interesting year due to the Covid-19 pandemic) and 2024. The main steps are:

- **Data Selection & Cleaning:**  
  - Selection of relevant columns from the datasets.
  - Data type conversion and handling of missing values.
  - Outlier removal using a mean + 7*std rule (especially for property values).
  - Harmonization of postal codes and assignment of regions to each department.

- **Comparative Analysis:**  
  - Number of transactions by region and property type.
  - Average price per square meter by region and property type.
  - Distribution of transactions by month and region.
  - Analysis of property types and crop types.

- **Visualization:**  
  - Bar and pie charts for property type and region distributions.
  - Line plots for price evolution over time.
  - Interactive maps (Folium) showing average property values by region.
  - Scatter plots for property value distributions over the year.

## Data Used

- `ValeursFoncieres-2020.txt`: Real estate transactions for 2020
- `ValeursFoncieres-2024.txt`: Real estate transactions for 2024
- `regions.geojson`: French regions boundaries (https://france-geojson.gregoiredavid.fr/)

## Main Libraries

- pandas, numpy: data processing
- matplotlib, seaborn, plotly: visualization
- folium: interactive mapping

## How to Run

1. Place the data files (`.txt` and `.geojson`) in the same folder as the notebook.
2. Open `Python_Data_Analysis.ipynb` in Jupyter or VS Code.
3. Run the cells in order.

## Key Results

- The regions with the highest number of properties in 2020 experienced a decrease in 2024, while regions with fewer properties in 2020 showed growth in 2024, likely due to the Covid-19 pandemic.
- The average price per square meter varies significantly by region and property type.
- The distribution of property types and crop types is visualized and compared between years.
- Interactive maps display the spatial distribution of property values.

## Author

Project carried out as part of a data analysis on French land values.