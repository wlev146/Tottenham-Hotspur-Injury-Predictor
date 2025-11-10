# Tottenham Hotspur Injury Predictor

### Predicting player injuries before they happen — using data, intuition, and storytelling

---

## Overview
This project explores how player workload, recovery time, and past injuries contribute to the likelihood of new injuries for **Tottenham Hotspur** players. Using a **logistic regression model**, I set out to answer:  
> *Can we predict when a player is at risk — before they actually get injured?*

The result was both technical and human. My final model successfully **predicted 7 new injuries before they occurred**, identifying elevated risk profiles days in advance. What began as a passion project became a lesson in the intersection of analytics, preparation, and performance.

---

## Goals
- Understand which factors most strongly influence injury risk (minutes, rest days, prior injuries, fixture congestion).  
- Engineer rolling workload metrics to reflect player fatigue more realistically.  
- Build and test a **logistic regression model** to classify injury risk.  
- Use **Power BI dashboards** to visualize injury likelihoods and communicate patterns effectively.  
- Tell a story that merges **data science and sports intuition** — showing how numbers can inform real-world decision-making.

---

## Dataset
I built the dataset from multiple public sources, including **FBref** and **Kaggle**, combining:  
- Player match logs (minutes played, position, opponent)  
- Injury records (dates, types, durations)  
- Rolling features (e.g., 7-day minute totals, 14-day minute totals)  
- Rest days between matches  
- Contextual match data (fixture congestion, competition type)

All preprocessing, cleaning, and feature engineering were done in **Python** using Pandas and PySpark.

---

## Process
1. **Data Cleaning** — Standardized names, corrected date inconsistencies, and filtered non-league matches.  
2. **Feature Engineering** — Created rolling workload metrics and rest-day variables to simulate fatigue cycles.  
3. **EDA (Exploratory Data Analysis)** — Explored visual correlations between workload, position, and injury frequency.  
4. **Modeling** — Built a **logistic regression classifier** to predict binary outcomes (injury / no injury).  
5. **Validation** — Cross-checked model output against real-world injury timelines.  
6. **Visualization** — Built **Power BI dashboards** showing risk trends by player, time period, and workload.

---

## Key Findings
- The model **predicted 7 new injuries before they actually occurred**, signaling risk spikes several days prior.  
- Players with **under 4 days of rest** had the highest predicted injury probability.  
- **Cumulative minutes** and **recent injury history** were strong predictors of future injury.  
- Positional trends showed higher risk for **wingers and fullbacks**, who often play high-intensity minutes.  
- While not perfect, the model
