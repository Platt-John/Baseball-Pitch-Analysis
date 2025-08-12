# ⚾ Baseball Pitch Analysis

## 📌 Overview
The goal of this project is to figure out the **top predictors of the start speed (in mph)** of an MLB pitch between 2015 and 2018, considering factors such as pitch location, acceleration, spin direction, and spin rate.
This project enables future coaches and MLB pitchers to understand better about how they can improve their in-game performance. I was motivated to do this project because of my desire to perform 
analysis on a large-scale dataset in addition to my interest in Sports Analytics in general.
## 📊 Data
- **Source:** [Kaggle – MLB Pitch Data 2015–2018](https://www.kaggle.com/datasets/pschale/mlb-pitch-data-20152018)
- **Description:** Metadata on every MLB pitch thrown from 2015–2018 (variables include `end_speed`, `spin_rate`, `spin_dir`, `zone`, `pitch_type`, etc.).
- **Target Variable:** `start_speed`
- **Size:** ~3 million rows × 40 columns, spanning 2015–2018

## 🛠️ Methods
- **Data Cleaning & Preprocessing:** Missing value handling, categorical encoding
- **Exploratory Data Analysis:** Bar charts, histograms, scatterplots
- **Statistical Analysis:** Violin plots, boxplots, t-tests
- **Predictive Modeling:** Simple & multiple linear regression

## 🛠️ Setup
1. Install [RStudio](https://posit.co/download/rstudio-desktop/).
2. Download:
   - `pitches.csv` dataset from Kaggle (link above)
   - `platt_finalproject.rmd` code file
3. Place both files in the same folder and set it as your working directory in RStudio.
4. Install required packages:
   ```r
   install.packages(c(
     "tidyverse", "tidymodels", "GGally", "stringr", 
     "ggfortify", "ggthemes", "ggmap", "sp", "rworldmap", "gapminder"
   ))
5. In RStudio:
- Click **Run** → **Run All**
- Knit to HTML via **Knit** icon

6. If errors occur:
- Verify all packages are installed
- Confirm `pitches.csv` is in the working directory
- Address any error messages

## 📈 Results
Top predictors of pitch start speed:
- Year of pitch
- Initial spin rate
- Initial horizontal acceleration
- Zone of the batter’s box where the pitch crosses home plate

## 📌 Future Work
Potential next steps:

- Predict **pitch type** for future MLB games
- Model **pitch location** given prior data
- Predict **number of baserunners** present when a pitch is thrown
- Integrate **more recent pitch data** for updated insights
