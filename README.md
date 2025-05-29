
# Heart Failure Clinical Analysis: Predictive Insights for Patient Outcomes

## Project Background

This analysis focuses on a comprehensive clinical dataset containing heart failure patient records from a healthcare system. As a data analyst working within the healthcare analytics team, I examined critical patient biomarkers and demographic factors to understand survival patterns and identify key risk indicators for heart failure mortality.

Heart failure affects millions of patients globally, with survival rates heavily dependent on early intervention and proper risk stratification. This analysis provides data-driven insights to support clinical decision-making and improve patient care protocols.

**Insights and recommendations are provided on the following key areas:**

- **Patient Demographics & Survival Patterns**: Gender, age, and overall mortality trends
- **Clinical Biomarkers Impact**: Laboratory values and their correlation with patient outcomes  
- **Risk Factor Analysis**: Comorbidities and lifestyle factors affecting survival rates
- **Predictive Indicators**: Key metrics for early intervention strategies


An interactive Tableau dashboard used to explore patient survival trends and clinical patterns can be found [here](https://public.tableau.com/views/HeartFailurePrediction_17447302203070/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

## Data Structure & Initial Checks

The clinical database consists of a single comprehensive table containing **299 patient records** with 13 key variables tracking patient demographics, clinical measurements, and outcomes. The dataset structure is as follows:

![Screenshot 2025-05-29 154421](https://github.com/user-attachments/assets/ccab76dc-64b6-4358-9199-7142ea264c33)

**Heart Failure Clinical Records Table:**
- **Patient Demographics**: Age, Sex  
- **Clinical Biomarkers**: Creatinine Phosphokinase, Ejection Fraction, Platelets, Serum Creatinine, Serum Sodium
- **Comorbidity Indicators**: Anaemia, Diabetes, High Blood Pressure, Smoking Status
- **Outcome Variables**: Time (follow-up period), Death Event (survival status)

*Total Records: 299 patients*  
*Follow-up Period: Variable (0-300 days)*  
*Overall Mortality Rate: 32.1% (96 deaths out of 299 patients)*

## Executive Summary

### Overview of Findings

This analysis reveals critical patterns in heart failure patient outcomes, with age and specific clinical biomarkers serving as the strongest predictors of mortality. Male patients demonstrate higher mortality rates (35.2%) compared to females (25.7%), while patients over 60 show significantly elevated risk profiles. Most importantly, ejection fraction emerges as the most reliable predictor, with patients having ejection fraction below 30% showing substantially higher mortality rates.


![Screenshot 2025-05-29 153239](https://github.com/user-attachments/assets/0d01e0ca-2008-48f6-8819-cfcf18c5c50c)

## Insights Deep Dive

### Patient Demographics & Survival Patterns

**Age Distribution Impact**: The patient population shows a clear age-related mortality pattern, with the highest death rates occurring in patients aged 60-80. Patients under 50 demonstrate notably better survival outcomes, with mortality rates below 20%.

**Gender-Based Survival Differences**: Male patients exhibit a 35.2% mortality rate compared to 25.7% for female patients, representing a 37% higher risk for male patients. This gender disparity suggests the need for more aggressive monitoring protocols for male heart failure patients.

**Population Demographics**: The study population averaged 60.8 years old, with a relatively balanced gender distribution (194 males, 105 females), providing robust statistical power for gender-based analysis.

**Time-to-Event Patterns**: Most deaths occurred within the first 100 days of follow-up, indicating a critical early intervention window for newly diagnosed or hospitalized heart failure patients.

### Clinical Biomarkers Impact

**Ejection Fraction as Primary Predictor**: Patients with ejection fraction values below 30% show dramatically higher mortality rates. The dashboard reveals a clear inverse relationship between ejection fraction and survival, making this the most critical metric for risk stratification.

**Serum Creatinine Elevation**: Elevated serum creatinine levels (>2.0 mg/dL) correlate strongly with poor outcomes, indicating kidney dysfunction as a significant comorbidity affecting heart failure prognosis.

**Creatinine Phosphokinase Trends**: While most patients show normal CPK levels, those with significantly elevated values (>1000) demonstrate higher mortality rates, suggesting cardiac muscle damage as a key factor.

**Platelet Count Variations**: Platelet counts outside the normal range (both high and low) correlate with increased mortality, potentially indicating underlying inflammatory processes or medication effects.

### Risk Factor Analysis

**Diabetes Mellitus Impact**: Diabetic patients show a mortality rate of 38.5% compared to 28.4% for non-diabetic patients, representing a 35% increase in relative risk and highlighting the importance of integrated diabetes-cardiac care.

**Smoking History Correlation**: Current or former smokers demonstrate elevated mortality rates, with the survival analysis showing clear separation between smoking and non-smoking cohorts throughout the follow-up period.

**Anaemia Prevalence**: Patients with anaemia show significantly worse outcomes, with mortality rates approaching 45% compared to 28% in non-anaemic patients, emphasizing the importance of treating concurrent anaemia.

**Hypertension Paradox**: Interestingly, patients with documented high blood pressure show slightly better survival rates, possibly due to more intensive medical management and monitoring.

### Predictive Indicators

**High-Risk Profile Identification**: Patients presenting with ejection fraction <30%, serum creatinine >1.5, age >65, and male gender represent the highest-risk cohort requiring immediate intensive intervention.

**Early Warning Indicators**: The combination of declining ejection fraction, rising creatinine, and presence of anaemia serves as a powerful early warning system for clinical deterioration.

**Survival Probability Factors**: Patients with ejection fraction >45%, normal kidney function, and absence of diabetes show survival rates exceeding 85%, indicating excellent prognosis with appropriate management.

**Critical Intervention Window**: The steep mortality curve in the first 90 days suggests that intensive monitoring and intervention during this period could significantly improve outcomes.

## Recommendations

Based on the insights and findings above, we would recommend the **Clinical Care Team and Hospital Administration** to consider the following:

**Enhanced Risk Stratification Protocol**: Implement an automated risk scoring system using ejection fraction, serum creatinine, age, and gender to immediately identify high-risk patients upon admission or diagnosis.

**Gender-Specific Care Pathways**: Develop specialized monitoring protocols for male heart failure patients, including more frequent follow-ups and earlier intervention thresholds given their 37% higher mortality risk.

**Integrated Diabetes-Cardiac Care**: Establish coordinated care protocols between cardiology and endocrinology teams for diabetic heart failure patients, given their significantly elevated mortality risk (38.5% vs 28.4%).

**Early Intervention Program**: Create an intensive 90-day post-diagnosis monitoring program, as the majority of deaths occur within this critical window, focusing on medication optimization and lifestyle intervention.

**Biomarker Monitoring Dashboard**: Implement real-time clinical dashboards tracking ejection fraction trends, kidney function, and anaemia status to trigger automated clinical alerts for deteriorating patients.

## Assumptions and Caveats

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

**Missing Follow-up Data**: Patients with incomplete follow-up periods were included in survival analysis up to their last known contact date, which may underestimate long-term survival rates for some cohorts.

**Comorbidity Coding**: Binary indicators for conditions like diabetes and hypertension assume consistent diagnostic criteria across the healthcare system, though actual severity levels may vary significantly between patients.

**Laboratory Value Standardization**: Clinical laboratory values were assumed to be measured using consistent methodologies and reference ranges, though different lab facilities may have slight variations in normal ranges and measurement techniques.

**Medication Effects Not Captured**: The analysis does not account for specific heart failure medications (ACE inhibitors, beta-blockers, diuretics) which could significantly impact survival outcomes and may confound some of the observed biomarker relationships.

**Single-Center Limitations**: Results may not be generalizable to other healthcare systems or patient populations with different demographic characteristics, access to care, or treatment protocols.
