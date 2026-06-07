# Group F — RMDS Hackathon

## Overview

This repository contains the code, data, and predictions produced by Group F as part of the
**Research Methods in Data Science (RMDS) Hackathon**.

The objective was to predict whether a survey respondent received a **seasonal flu vaccine**
(`seasonal_vaccine`, binary target), using a dataset of 30 behavioural, attitudinal, and
demographic features. Five machine learning models were trained, evaluated, and ranked by
F1 score, with final predictions compiled into a submission CSV.

---

## Dataset

The dataset contains **31 columns**: a unique `respondent_id` and 30 feature variables.

### Feature Categories

| Category              | Features                                                                                                                                                          |
|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Flu concern & knowledge | `flu_concern` (0–3), `flu_knowledge` (0–2)                                                                                                                      |
| Behavioural indicators  | `behavioral_antiviral_meds`, `behavioral_avoidance`, `behavioral_face_mask`, `behavioral_wash_hands`, `behavioral_large_gatherings`, `behavioral_outside_home`, `behavioral_touch_face` (all binary) |
| Health & medical        | `doctor_recc_seasonal`, `chronic_med_condition`, `child_under_6_months`, `health_worker`, `health_insurance` (all binary)                                       |
| Vaccine opinions        | `opinion_seas_vacc_effective`, `opinion_seas_risk`, `opinion_seas_sick_from_vacc` (ordinal, 1–5)                                                                |
| Demographics            | `age_group`, `education`, `race`, `sex`                                                                                                                         |
| Socioeconomic           | `income_poverty`, `marital_status`, `rent_or_own`, `employment_status`, `census_msa`, `household_adults`, `household_children`, `employment_sector`            |

**Target variable:** `seasonal_vaccine` — `0` = did not receive, `1` = received

---

## Models Compared

Five classifiers were implemented and evaluated. Predictions were submitted in a CSV ordered
by F1 score ranking:

1. **XGBoost**
2. **CatBoost**
3. **LightGBM**
4. **Decision Tree**
5. **Random Forest**

---

## Team Breakdown

The team was split into three sub-groups, each responsible for implementing specific models.

### Sub-group 1 — Srikavya & Navaneeth
**Models:** XGBoost, CatBoost

### Sub-group 2 — Sunday & Rishitha
**Models:** LightGBM, Decision Tree

### Sub-group 3 — Anjireddy & Tharun
**Models:** Random Forest

---
