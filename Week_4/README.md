# AnalystLab Data Analytics Internship
## Week 4 - HealthConnect Experience 
## Initial Analysis & Project Planning

## **Project Overview**

The **HealthConnect Experience Lab** is a healthcare analytics project designed to explore how data can be used to improve appointment attendance, operational efficiency, and patient support.

HealthConnect Clinic is experiencing challenges including missed appointments, inefficient use of appointment slots, difficulty identifying factors associated with no-shows, and repetitive patient enquiries relating to appointments and clinic procedures.

The central business question for the project is:

**How can HealthConnect Clinic use data to reduce missed appointments and improve the patient support experience?**

As a **Data Analytics Intern**, my role in Week 4 was to understand the business problem, review the available appointment data, assess data quality, identify variables relevant to appointment attendance, define meaningful business questions and KPIs, and establish an initial analytical approach for subsequent stages of the project.

## Week 4 Objectives

The main objectives of this stage were to:

- Understand the HealthConnect business problem.
- Review the structure and content of the appointment dataset.
- Examine the provided data dictionary.
- Conduct an initial data quality assessment.
- Identify variables relevant to appointment attendance and no-shows.
- Define business questions that can be investigated using the data.
- Identify potential KPIs for future analysis.
- Consider assumptions, limitations, risks, and dependencies.
- Establish an initial analytical approach for the next phase of the project.

## Business Scenario

HealthConnect Clinic manages appointment-based healthcare services and wants to improve the way appointment data is used to support operational and patient-related decision-making.

Key challenges identified include:

1. Patients missing scheduled appointments.
2. Difficulty understanding patterns associated with appointment no-shows.
3. Inefficient utilisation of appointment slots.
4. Repetitive patient enquiries concerning appointments and clinic procedures.
5. The need to improve patient engagement and administrative support.

The project therefore focuses on using data to understand appointment outcomes and identify actionable patterns that could support better decision-making.

## Dataset

### HealthConnect Appointment Dataset

**File:** `HealthConnect_Appointment_Data.csv`

The dataset contains **5,000 appointment records** across **18 variables**.

The variables cover several areas:

- Patient demographics
- Appointment information
- Booking information
- Previous appointment history
- Previous no-shows
- Reminder information
- Distance to clinic
- Waiting time
- Appointment outcomes

### Data Dictionary

**File:** `HealthConnect_Data_Dictionary.xlsx`

The data dictionary was reviewed to understand the meaning, data type, and expected use of each variable in the appointment dataset.

## Dataset Structure

The dataset contains the following major variable groups:

1. Patient Information: Patient ID, Gender, Age, Age Group 
2. Appointment Information: Appointment Type, Appointment Date, Appointment Day, Appointment Time 
3. Booking Information: Booking Date, Booking Lead Days 
4. Appointment History: Previous Appointments, Previous No-Shows 
5. Reminder Information: Reminder Sent, Reminder Channel 
6. Operational Information: Distance to Clinic, Waiting Time 
7. Outcome: Appointment Outcome 

The primary outcome variable for future analysis is:

**`appointment_outcome`** with categories including:

- Attended
- No-Show
- Cancelled

## Initial Data Quality Assessment

An initial review of the dataset was conducted to identify missing values, potential data quality issues, data types, and variables requiring further validation.

### Dataset Profile

- **Total records:** 5,000
- **Total variables:** 18
- **Distance to Clinic missing values:** 90
- **Waiting Time missing values:** 60

The missing values identified in these two variables will need to be assessed further before analysis.

### Reminder Channel

The `reminder_channel` variable contains:

- SMS
- Email
- WhatsApp
- None

## Key Business Questions

The following questions were identified for subsequent analysis:

### Appointment Attendance

1. What proportion of appointments result in a no-show?
2. Which appointment types have the highest no-show rates?
3. Are certain age groups more likely to miss appointments?
4. Does appointment timing influence attendance?
5. Are certain days of the week associated with higher no-show rates?

### Patient Behaviour

6. Does previous no-show history relate to future appointment attendance?
7. Does the number of previous appointments influence attendance?
8. Is booking lead time associated with no-show behaviour?

### Reminder Effectiveness

9. Does receiving an appointment reminder affect attendance?
10. Which reminder channels are associated with better attendance outcomes?

### Operational Factors

11. Does distance to the clinic relate to appointment attendance?
12. Is waiting time associated with appointment outcomes?
13. Which appointment categories experience the greatest potential loss from missed appointments?

## Potential KPIs

The following KPIs were identified for future analysis:

**No-Show Rate** Measures the overall scale of missed appointments. 
**Attendance Rate** Tracks appointment attendance performance. 
**Cancellation Rate** Helps assess appointment utilisation. 
**Reminder Effectiveness Rate** Evaluates the potential value of reminder interventions.
**Previous No-Show Rate** Helps identify patients requiring additional engagement. 

These KPIs are proposed for future stages and were not treated as final calculated results during Week 4.

## Initial Analysis Approach

The proposed analytical workflow for subsequent stages is:

### 1. Data Understanding
Review the dataset structure and data dictionary to understand the variables and their business meaning.

### 2. Data Quality Assessment
Identify and document:

- Missing values
- Duplicate records
- Incorrect data types
- Inconsistent categorical values
- Invalid dates
- Potential outliers
- Unexpected values

### 3. Data Cleaning and Transformation
Prepare a separate cleaned version of the dataset without altering the original project resource.

Potential transformations may include:

- Standardising categorical values
- Correcting data types
- Handling missing values appropriately
- Validating date fields
- Creating analytical categories where necessary
- Checking duplicate appointment records

### 4. Exploratory Data Analysis

Analyse appointment outcomes against relevant factors, including:

- Age and age group
- Gender
- Appointment type
- Appointment day
- Appointment time
- Booking lead days
- Previous appointments
- Previous no-shows
- Reminder status
- Reminder channel
- Distance to clinic
- Waiting time

### 5. KPI Development

Calculate and evaluate the selected KPIs to quantify appointment attendance and no-show patterns.

### 6. Visual Analytics

Develop appropriate visualisations using tools such as **Power BI, Python, or SQL** to communicate patterns and support decision-making.

### 7. Business Recommendations

Translate analytical findings into practical recommendations that could help HealthConnect reduce missed appointments and improve patient engagement.

## Tools & Technologies

The Data Analytics track may utilise:

- **Microsoft Excel** — initial data inspection and preparation
- **Power Query** — data cleaning and transformation
- **SQL** — data querying and analysis
- **Power BI** — data visualisation and dashboard development

Tools will be selected based on the requirements of each project stage.

## Assumptions

The following assumptions apply to the initial analysis:

- The dataset is fictional and anonymised.
- `appointment_id` is treated as the unique appointment identifier.
- `patient_id` may occur across multiple appointment records.
- `appointment_outcome` is the primary outcome variable for attendance analysis.
- `None` in `reminder_channel` represents no reminder channel rather than missing information.
- Missing values will be assessed based on the meaning of each variable rather than automatically removed.
- The original project dataset will not be overwritten.

## Limitations

Initial limitations identified include:

- The dataset is fictional and may not represent real-world healthcare behaviour.
- Some variables contain missing values.
- The dataset does not necessarily capture every factor that may influence appointment attendance.
- Observed relationships may not establish causation.
- Distance and waiting-time values contain limited missing observations.
- The dataset provides limited contextual information about patient circumstances.
- Further validation is required before drawing final business conclusions.

## Risks & Dependencies

Potential project risks and dependencies include:

- Incorrect handling of missing values could affect analysis.
- Inconsistent categorical values could produce misleading results.
- Data quality issues may affect KPI calculations.
- Conclusions depend on the reliability and completeness of the provided dataset.
- Further project stages depend on successful data cleaning and validation.
- Recommendations should remain within the evidence provided by the dataset and should not introduce unsupported medical assumptions.

## Week 5 Focus

The next stage of the project will build upon the Week 4 foundation.

The proposed focus is to:

- Perform detailed data cleaning.
- Validate data types and categorical values.
- Investigate duplicates and missing values.
- Conduct exploratory data analysis.
- Analyse appointment attendance and no-show patterns.
- Calculate the selected KPIs.
- Identify significant patterns and potential churn/no-show drivers.
- Begin developing analytical outputs that can support the broader HealthConnect solution.

**Created By**

**Chidiebere Lilian Ebulue**

**AnalystLab Africa**
