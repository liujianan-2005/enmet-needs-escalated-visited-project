# Unmet Needs and Escalated Care Analysis

## Project Overview

This project analyzes patient encounter data and social determinants of health survey data from a healthcare system to investigate whether unmet basic needs are associated with escalated care journeys.

The analysis focuses on whether patients experiencing social barriers such as food insecurity, transportation difficulties, housing instability, or financial strain are more likely to experience emergency visits or hospital admissions.

---

## Research Question

Are patients with unmet basic needs more likely to experience escalated care journeys, defined by emergency visits or hospital admissions?

---

## Datasets

The project uses two primary datasets:

### encounters.csv
Contains detailed records of patient interactions with the Stormont Vail Health (SVH) system from January 2022 to December 2025.

### social_determinants.csv
Contains survey-based information on social and environmental factors that may influence patients’ health. Each row corresponds to a response to a specific question asked during a patient encounter.

Due to privacy and data-sharing restrictions, the original healthcare datasets are not publicly available.

---

## Methods

The analysis workflow includes:

1. Identifying survey questions associated with different categories of unmet basic needs
2. Constructing patient-level unmet need indicators based on survey responses
3. Aggregating the total number of unmet needs for each patient
4. Creating escalated care indicators based on emergency visits or hospital admissions
5. Determine the number of escalated visits and having escalated visits or not for each patinet
6. Merging escalated visits and unmet needs datasets using patientDurableKey
7. Performing exploratory analysis and binomial logistic regression modeling

---

## Results

Binomial logistic regression analysis identified a statistically significant positive relationship between unmet social needs and escalated care occurrence (p = 0.0012).

The model estimated that each additional unmet need increased the odds of experiencing escalated care by approximately 65%.

These findings suggest that patients experiencing greater unmet social needs may be more likely to experience emergency visits or hospital admissions.

---

## Tools and Technologies

- R
- tidyverse
- dplyr
- ggplot2
- Jupyter Notebook

---

## Repository Structure

```text
workpage.ipynb     # Main analysis notebook
README.md          # Project overview
