# HealthConnect Clinic – Week 5 Data Analytics Project

## AnalystLab Africa

### Exploratory Data Analysis, KPI Development & Business Insights

## Project Overview

This project represents my Week 5 contribution to the **AnalystLab Africa HealthConnect Experience Lab** as a Data Analytics Intern.

HealthConnect Clinic is a fictional healthcare provider that manages appointment-based services and is experiencing challenges related to missed appointments, patient engagement, and efficient utilisation of appointment slots.

The central business question guiding this project is:

**How can HealthConnect Clinic use data to reduce missed appointments and improve the patient support experience?**

Week 4 focused on understanding the business problem, reviewing the available resources, assessing data quality, identifying relevant business questions, and proposing potential KPIs.

Week 5 builds directly on that foundation by moving from planning into practical implementation through:

- Data preparation and quality assessment
- Exploratory Data Analysis (EDA)
- KPI development and calculation
- Power BI analytical dashboard development
- Identification of business insights
- Business recommendations
- Documentation of assumptions, limitations, risks and dependencies
- Cross-track collaboration considerations

# Project Objectives

The main objectives of this project were to:

1. Analyse appointment attendance and no-show patterns.
2. Identify factors associated with missed appointments.
3. Examine relationships between patient, appointment and operational characteristics and appointment outcomes.
4. Develop meaningful KPIs for monitoring appointment performance.
5. Build an interactive Power BI analytical dashboard.
6. Translate analytical findings into actionable business insights.
7. Recommend practical actions that HealthConnect Clinic can consider to reduce missed appointments and improve appointment operations.

# Dataset

### Dataset Used

**HealthConnect Appointment Dataset**

The dataset contains fictional appointment records covering information such as:

- Patient characteristics
- Appointment details
- Appointment outcomes
- Appointment timing
- Previous appointment history
- Previous no-shows
- Reminder information
- Waiting time
- Distance to clinic
- Cancellation information

The accompanying **HealthConnect Data Dictionary** was used as a reference for understanding the meaning and expected interpretation of dataset variables.

**Important:** The original project dataset was preserved and was not overwritten. Any cleaned or transformed data was handled separately.

# Data Preparation & Quality Assessment

Before conducting the analysis, the dataset was reviewed to assess its structure and quality.

The preparation process included:

- Reviewing dataset structure and variables
- Checking data types
- Checking for missing values
- Checking for duplicate records
- Reviewing categorical values for consistency
- Examining numerical fields for unusual values
- Creating analytical groups where appropriate
- Documenting relevant data-quality issues

### Key Data-Quality Observations

Some missing values were identified in operational variables, including:

- **Waiting Time:** 60 blank records
- **Distance to Clinic:** 90 blank records

These missing observations were considered when interpreting the corresponding analyses.

### Booking Lead Time

The dataset contained negative values in the Booking Lead Time field.

Because these values could result in misleading interpretations, Booking Lead Time was excluded from the Week 5 analytical dashboard rather than introducing unsupported assumptions.

# Exploratory Data Analysis

The EDA focused on identifying patterns and relationships that could help HealthConnect understand and reduce appointment no-shows.

The analysis covered the following areas:

### Appointment Characteristics

- Appointment type
- Appointment time
- Appointment day
- Appointment outcome
- Cancellation patterns

### Patient Characteristics

- Age groups
- Patient demographics
- Distance to clinic

### Previous Appointment History

- Previous no-shows
- Relationship between previous attendance behaviour and future no-shows

### Reminder Information

- Reminder coverage
- Reminder channel
- Relationship between reminders and appointment outcomes

### Operational Factors

- Waiting time
- Distance to clinic
- Appointment timing
- Cancellation rate

The analysis was designed around practical business questions rather than producing visuals without a clear decision-making purpose.

# Key Performance Indicators (KPIs)

Four KPIs were selected for Week 5 based on their relevance to the HealthConnect business problem.

No-Show Rate 
Cancellation Rate
Reminder Coverage 
Average Waiting Time 

These KPIs provide a high-level view of appointment attendance, patient engagement and operational performance.

# Power BI Dashboard

An interactive Power BI dashboard was developed to communicate the results of the exploratory analysis.

The dashboard consists of three analytical pages.

## 1. Executive Appointment Overview

This page provides a high-level view of appointment performance.

### Key areas covered:

- No-show rate
- Cancellation rate
- Reminder coverage
- Average waiting time
- Appointment outcomes
- No-show rate by appointment type
- No-show rate by appointment day
- No-show rate by reminder channel
- Appointment volume trends

### Purpose

The Executive Appointment Overview allows users to quickly understand the overall appointment situation and identify major areas requiring attention.

## 2. No-Show Drivers

This page focuses specifically on factors associated with missed appointments.

### Key analyses include:

- No-show rate by age group
- No-show rate by appointment type
- No-show rate by appointment time
- No-show rate by distance group
- Previous no-shows versus future no-show behaviour
- Appointment characteristics associated with higher no-show rates

### Purpose

The page helps identify patient and appointment segments that may require targeted engagement or additional appointment support.

## 3. Patient Support & Appointment Operations

This page examines operational factors that may influence appointment attendance and patient experience.

### Key analyses include:

- Appointment outcomes by reminder channel
- Appointment outcomes by appointment time
- Cancellation rate by appointment type
- Waiting-time analysis
- Appointment operational patterns

### Purpose

The page supports operational decision-making by highlighting areas where patient communication, reminder processes and appointment management could potentially be improved.

# Key Business Insights

The analysis produced several important observations.

### 1. High overall no-show rate

The overall no-show rate was **48.5%**, indicating that almost half of recorded appointments were missed.

This represents a significant opportunity for HealthConnect to improve appointment utilisation and patient engagement.

### 2. Previous no-shows are associated with future no-shows

No-show rates increased across patients with higher numbers of previous no-shows, with the highest observed rate occurring among the small group with five previous no-shows.

This suggests that previous attendance behaviour may be useful when identifying patients who could benefit from additional appointment support.

### 3. Distance may influence appointment attendance

Patients in the **21+ km distance group recorded the highest no-show rate at 57.8%**.

This suggests that travelling distance may represent a potential accessibility factor that should be considered when designing patient engagement strategies.

### 4. Reminder coverage remains an important operational consideration

Approximately **72.7% of appointments received a recorded reminder**, while appointments without a recorded reminder had a higher observed no-show rate than several reminder channels.

This indicates an opportunity to review reminder coverage and channel effectiveness.

### 5. Follow-up appointments recorded the highest no-show rate

Follow-up appointments recorded a no-show rate of approximately **51.2%**, higher than the other appointment types analysed.

This suggests that follow-up appointments may require additional investigation and potentially more targeted patient communication.

These findings represent observed relationships within the dataset and should not automatically be interpreted as causal relationships.

# Business Risks

The analysis highlights several potential business risks:

### Appointment Slot Underutilisation

A high no-show rate may result in unused appointment capacity and reduced operational efficiency.

### Patient Engagement Risk

Repeated missed appointments may indicate that certain patient groups require stronger communication, reminders or appointment support.

### Accessibility Risk

Higher no-show rates among patients travelling longer distances may indicate potential accessibility or transportation-related barriers.

# Business Opportunities

The analysis also identifies opportunities for HealthConnect to:

- Improve reminder coverage and communication strategies.
- Identify patients with previous no-show behaviour for targeted engagement.
- Review appointment management for higher-risk appointment types.
- Provide additional support to patients travelling longer distances.
- Use appointment data to continuously monitor attendance patterns.

# Business Recommendations

Based on the findings, the following actions are recommended:

1. **Increase reminder coverage** by ensuring eligible appointments receive timely reminders.

2. **Develop targeted engagement for patients with previous no-shows**, using historical attendance behaviour as a risk indicator.

3. **Evaluate reminder channels** to determine which communication methods are most effective for different patient groups.

4. **Investigate the higher no-show rate among follow-up appointments** and consider additional confirmation or engagement strategies.

5. **Provide additional support for patients travelling longer distances**, such as earlier reminders, confirmation calls or flexible scheduling where operationally feasible.

6. **Establish continuous KPI monitoring** using no-show rate, cancellation rate, reminder coverage and waiting time.

# Cross-Track Collaboration

HealthConnect is designed as a multidisciplinary project involving different professional tracks.

From a Data Analytics perspective, the outputs generated during Week 5 can support other tracks, particularly **Data Science, Machine Learning and Generative AI**.

Potential analytical outputs that can be shared include:

- No-show rate
- Previous no-show behaviour
- Reminder information
- Appointment characteristics
- Patient segmentation variables
- Distance and waiting-time patterns

These findings can help other tracks identify relevant features, define potential prediction targets and design patient-support solutions.

Where applicable, actual collaboration and exchanged outputs should be documented based on the interaction completed during the internship.

# Assumptions, Limitations, Risks & Dependencies

### Assumptions

- The dataset represents fictional and anonymised HealthConnect appointment records.
- Appointment outcomes are assumed to accurately represent the recorded appointment status.
- Grouped variables such as Age Group and Distance Group are used for analytical comparison.
- Observed relationships are treated as associations rather than confirmed causal relationships.

### Limitations

- Missing values exist in Waiting Time and Distance to Clinic.
- The dataset contains questionable Booking Lead Time values, including negative values.
- The dataset is fictional and may not fully represent real-world healthcare operations.
- Some categories may contain relatively small numbers of observations.
- The analysis does not establish causation.

### Risks

- Poor data quality could affect analytical accuracy.
- Over-interpreting correlations could result in inappropriate business decisions.
- Small sample groups may produce unstable rates.

### Dependencies

Future stages may depend on:

- Improved data-quality controls
- Validated appointment records
- Additional operational information
- Collaboration with Data Science, Machine Learning or other project tracks
- Availability of reliable patient-support and appointment-management processes
  
# Tools & Technologies

The main tools used for this project include:

- **Power Query**
- **Microsoft Power BI**
- **DAX**
- **Microsoft Word**

### Power BI was used for:

- Data modelling
- KPI development
- Data analysis
- Interactive visualisation
- Dashboard development
- Business insight communication

### Power Query was used for:

- Data preparation
- Data-quality assessment
- Transformation and validation
- Preliminary inspection of the dataset

### Microsoft Word was used for:

- Report writing

###Created By

**Chidiebere Lilian Ebulue**

**AnalystLab Africa**
