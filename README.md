# 🫁 Health Intelligence — Lung Cancer: Diagnosis Patterns & Risk Stratification

> A end-to-end data analytics project investigating the behavioural, symptomatic, and demographic risk factors associated with lung cancer diagnosis. Built using Microsoft Power BI with custom DAX measures, interactive slicers, and a three-page stakeholder-ready dashboard.

---

<img width="1325" height="2428" alt="Health_Intelligence_Dashboard_reports" src="https://github.com/user-attachments/assets/fd8e42fd-7c9c-4161-be87-3d684d186795" />


---

## 📌 Project Background

Lung cancer remains one of the leading causes of cancer-related mortality worldwide. Despite advances in treatment, late-stage diagnosis continues to drive poor survival outcomes — making early identification of at-risk individuals a critical public health priority.

This project analyses a behavioural and demographic health survey dataset of **309 participants** to uncover the patterns, risk profiles, and predictive indicators most strongly associated with a lung cancer diagnosis. The analysis moves across four analytical dimensions — symptomatic, behavioural, demographic, and predictive risk — and consolidates findings into an interactive Power BI dashboard designed for both clinical and public health stakeholders.

This is the first project in the **Health Intelligence Portfolio Series** — a collection of healthcare analytics projects spanning disease diagnosis, patient risk stratification, and public health data.

---

## 🎯 Project Objectives

- Identify which physical symptoms appear most consistently across confirmed lung cancer diagnoses
- Quantify the relationship between substance use (smoking, alcohol) and diagnosis outcomes
- Determine whether psychosocial factors — anxiety, peer pressure — carry measurable diagnostic weight
- Validate a risk stratification model across High, Medium, and Low risk cohorts
- Produce actionable, evidence-based recommendations for clinical and public health application

---

## 📊 Dashboard Overview

The dashboard is structured across **three navigable pages**, each serving a distinct analytical purpose:

### Page 1 — Main Dashboard
The primary analytical view. Contains four KPI cards for headline metrics, and six interactive visuals covering symptom distribution, substance use correlation, risk tier breakdown, behavioural profiling, gender split, and age-band diagnosis rates. Three slicers — Lung Cancer status, Age Group, and Gender — enable dynamic cross-filtering across all visuals simultaneously.

### Page 2 — Observations
A dedicated narrative page translating the visual findings into written analytical observations. Eight structured observations cover symptom concentration, substance use correlation, behavioural risk flags, risk model validation, age-dependency, gender distribution, overall diagnosis rate, and average patient age.

### Page 3 — Recommendations
An evidence-based recommendations page converting the analytical findings into eight specific, actionable public health and clinical recommendations — from symptom-triggered screening protocols to age-gated lung health check policies.

---

## 📈 Key Metrics

| Metric | Value |
|---|---|
| Overall Diagnosis Rate | 87.38% |
| Total Participants | 309 |
| Confirmed Diagnoses | 270 |
| Average Age of Diagnosed | 63 years |
| Most Common Symptom | Fatigue (189 cases) |
| Leading Behavioural Risk Factor | Alcohol Consumption (165 diagnosed) |
| High Risk Diagnosis Rate | 100% (80/80) |
| Peak Age Group Diagnosis Rate | 98.04% (71–80 bracket) |

---

## 🗂️ Dataset

| Field | Detail |
|---|---|
| Source | Behavioural and Demographic Health Survey |
| Size | 309 participants |
| Format | CSV / Excel |
| Collection Method | Self-reported survey responses |

### Variables Included

**Demographic**
- Age Group
- Gender

**Behavioural & Psychological**
- Smoking Status
- Alcohol Consumption
- Anxiety
- Peer Pressure
- Chronic Disease

**Physical Symptoms**
- Fatigue
- Shortness of Breath
- Coughing
- Wheezing
- Chest Pain
- Yellow Fingers
- Swallowing Difficulty

**Outcome Variable**
- Lung Cancer Diagnosis (Yes / No)

---

## 🔧 Tools & Methodology

| Tool | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard development, data modelling, visualisation |
| DAX (Data Analysis Expressions) | Custom measures, KPI calculations, risk classification logic |
| Power Query | Data cleaning and transformation |

### Analytical Approach

The methodology combines two analytical modes:

**Descriptive Analytics** — understanding what the data shows through frequency distributions, KPI tracking, and demographic breakdowns.

**Diagnostic Analytics** — understanding why patterns exist through cross-tabulation, risk stratification, behavioural profiling, and correlation mapping.

### DAX Measures Built

- `Diagnosis Rate %` — total diagnosed as a proportion of all participants
- `Average Age of Diagnosed` — mean age scoped exclusively to confirmed cases
- `Risk Tier Classification` — conditional logic assigning High / Medium / Low risk based on cumulative indicator scores
- `Symptom Count by Diagnosis Status` — drives treemap proportional sizing
- `Behavioural Flag Totals` — aggregated counts per behaviour segmented by diagnosis outcome

---

## 📉 Dashboard Visuals Explained

| Visual | Chart Type | What It Shows |
|---|---|---|
| Symptom Distribution Among Diagnosed | Treemap | Proportional frequency of each symptom among confirmed cases. Fatigue dominates at 189 occurrences |
| Lung Cancer Diagnosis by Substance Usage | 100% Stacked Column | Side-by-side comparison of alcohol and smoking usage rates across diagnosed vs non-diagnosed participants |
| Risk Level Breakdown | Ribbon Chart | Distribution of Low, Medium, and High risk participants — with diagnosis overlay showing predictive accuracy of each tier |
| Behavioural Risk Matrix | Matrix Table | Cross-tabulation of five behavioural factors (smoking, alcohol, anxiety, peer pressure, chronic disease) against diagnosis status |
| Gender Distribution of Diagnosed Cases | Donut Chart | Male vs female split among the 270 confirmed diagnoses |
| Age Group vs Lung Cancer Diagnosis | 100% Stacked Bar | Diagnosis rates across seven age bands from 21–30 through to 81–90 |

---

## 🔍 Key Findings & Observations

### 1. Fatigue, Shortness of Breath & Coughing Are the Dominant Symptom Cluster
Fatigue (189), shortness of breath (176), and coughing (169) were the three most prevalent symptoms across confirmed diagnoses — appearing consistently across the majority of positive cases. These three symptoms form a clear primary triage cluster for clinical risk flagging.

### 2. Substance Use Shows Strong Correlation with Diagnosis
Of the 270 diagnosed participants, 155 reported smoking and 165 reported alcohol consumption. Both figures significantly exceed their non-diagnosed counterparts, establishing a strong statistical association between substance use behaviours and lung cancer diagnosis in this dataset.

### 3. Psychosocial Factors Emerge as Significant Risk Flags
145 diagnosed individuals reported experiencing peer pressure; 142 reported anxiety. Both ranked as the top behavioural traits among confirmed cases alongside chronic disease — suggesting that psychosocial stressors carry measurable diagnostic weight that is often underrepresented in purely clinical datasets.

### 4. The Risk Stratification Model Is Highly Predictive
The High Risk cohort achieved a **100% diagnosis rate (80/80)** — every participant classified as High Risk was confirmed with lung cancer. The Medium Risk tier reached 91.35%, while the Low Risk group showed a more balanced split (21 diagnosed, 23 not). This validates the stratification logic as a strong foundation for a clinical decision support tool.

### 5. Age Is a Hard Threshold Risk Factor
Participants under 40 recorded **zero diagnoses**. The 51–70 age band exceeded 85% diagnosis rates across all sub-groups, with the 71–80 bracket peaking at 98.04%. This establishes age 41 as a meaningful risk threshold — and suggests that screening protocols timed from age 50 would capture the vast majority of at-risk individuals.

### 6. Males Show Marginally Higher Prevalence
145 of 270 diagnosed cases were male (53.7%) versus 125 female (46.3%). The gap is modest but consistent — sufficient to justify gender-differentiated screening and public health messaging strategies.

### 7. The Overall Diagnosis Rate Signals a High-Risk Dataset
An 87.38% diagnosis rate across 309 participants is substantially higher than general population lung cancer prevalence. This reflects a purposefully sampled high-risk population — a methodological consideration that should be factored into how findings are applied beyond this dataset.

### 8. The Average Diagnosis Age of 63 Aligns with Global Trends
The mean age of confirmed diagnoses sits at 63 years — consistent with international epidemiological data confirming that lung cancer risk accelerates significantly from the sixth decade of life onward.

---

## ✅ Recommendations

### 1. Implement Symptom-Triggered Screening Protocols
Establish standardised early-detection pathways for patients presenting with fatigue, persistent cough, or shortness of breath. These three symptoms formed the dominant cluster across confirmed diagnoses and should serve as primary triage flags for pulmonary referral.

### 2. Integrate Substance Use into Clinical Risk Scoring
Clinical intake processes should systematically capture smoking history and alcohol consumption patterns. The strength of the correlation in this dataset supports embedding substance use as a weighted variable in automated risk scoring tools.

### 3. Embed Mental Health Indicators into Routine Health Screenings
Anxiety and peer pressure emerged as significant co-occurring factors among diagnosed individuals. Incorporating validated mental health screening questions into routine health assessments would enable earlier identification of psychosocially at-risk individuals.

### 4. Deploy a Predictive Risk Stratification System
The three-tier risk classification model demonstrated exceptional predictive power. A clinical decision support system built on this logic would allow healthcare providers to prioritise high-risk patients for urgent diagnostic screening — improving resource allocation and early detection rates.

### 5. Concentrate Preventive Care on the 50+ Age Bracket
With diagnosis rates exceeding 85% across the 51–80 cohort, preventive care investment — including subsidised screening programmes and targeted public health campaigns — should be concentrated on individuals aged 50 and above, particularly those presenting with additional risk factors.

### 6. Adopt Gender-Sensitive Public Health Messaging
Gender-targeted communication strategies, with particular focus on men aged 50 and above, can incrementally improve screening uptake and early diagnosis rates — even where the gender gap in prevalence is narrow.

### 7. Pursue Broader Dataset Diversity in Future Research
The 87.38% diagnosis rate indicates a non-representative, high-risk focused sample. Future survey design should target balanced case-to-control ratios to improve model generalisability and reduce sampling bias for population-wide application.

### 8. Standardise Lung Health Screening Entry at Age 50
Given the average diagnosis age of 63 and the steep escalation in risk from age 50 onward, clinical guidelines should consider mandating baseline lung health assessments at age 50 for individuals presenting with known risk factors such as fatigue, smoking history, or regular alcohol consumption.

---

## ⚠️ Limitations

- **Sampling Bias** — The 87.38% diagnosis rate indicates a non-representative, high-risk skewed sample. Findings should not be extrapolated to general population incidence without caution
- **Self-Reported Data** — Behavioural and symptomatic variables rely on participant self-reporting, introducing potential recall bias and social desirability effects
- **Cross-Sectional Design** — The dataset captures a single point in time. Causal relationships cannot be established — only correlational associations
- **Absent Clinical Variables** — Laboratory markers, imaging results, smoking pack-years, and full diagnostic history were not included. Their addition would significantly strengthen clinical applicability

---

## 🔭 Future Work

- Incorporate machine learning classification models (logistic regression, random forest, XGBoost) to move from descriptive and diagnostic analytics into predictive modelling
- Source a balanced dataset with equitable representation of diagnosed and non-diagnosed participants to enable robust model training and validation
- Add longitudinal tracking to examine how risk factor accumulation over time affects diagnosis probability
- Expand the variable set to include genetic markers, occupational exposure history, BMI, and socioeconomic indicators
- Build a clinical risk scoring tool in Python or R based on the stratification logic developed in this analysis

---

## 📁 Repository Structure
📦 Health-Analytics-Lung-Cancer-Diagnosis-and-Risk-Stratification

┣ 📊 Health_Intelligence_Lung_Cancer.pbix       ← Power BI dashboard file (open in Power BI Desktop)

┣ 📄 Lung_Cancer_Technical_Report.docx          ← Full technical report with methodology and findings

┣ 🖼️ Health_Intelligence_Dashboard.jpg          ← Dashboard preview image (displayed in this README)

┣ 📋 survey_lung_cancer.csv                     ← Raw dataset — 309 participants, 16 variables

┗ 📝 README.md                                  ← Project documentation (you are here)
