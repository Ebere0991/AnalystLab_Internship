# HealthConnect Clinic Experience Lab — Week 8 Final Analytics & Decision Support
## Analyst Lab Africa Internship 
## Data Analytics Track

## Project Overview

The HealthConnect Clinic Experience Lab project focused on exploring how data and AI can be used to improve healthcare appointment management and patient support.

The central project question was:

> **How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?**

As part of the Data Analytics track, my role was to analyse appointment and patient data, identify meaningful patterns associated with missed appointments, develop performance indicators, build Power BI dashboards, validate analytical findings, and translate the results into business insights and decision-support recommendations.

Week 8 represents the final stage of my Data Analytics contribution, bringing together the work completed across the previous weeks into a final analytics and decision-support package.

# Objectives

The Data Analytics contribution focused on:

- Understanding appointment attendance patterns.
- Preparing and analysing the HealthConnect appointment dataset.
- Developing meaningful KPIs for appointment performance.
- Building interactive Power BI dashboards.
- Investigating factors associated with missed appointments.
- Conducting deeper segment-level analysis.
- Testing and validating important analytical findings.
- Refining analytical outputs and supporting evidence.
- Translating findings into business insights and recommendations.
- Sharing relevant analytical evidence with other project tracks.
- Supporting the wider HealthConnect solution with an evidence-based analytics layer.
- Presenting the final Data Analytics contribution professionally.

# Dataset

The project used the **HealthConnect Appointment Dataset**, containing approximately **5,000 appointment records** and variables relating to patients, appointments, reminders, attendance outcomes and operational characteristics.

Key variables included:

- Appointment ID
- Patient ID
- Gender
- Age
- Age Group
- Appointment Type
- Booking Date
- Appointment Date
- Appointment Day
- Appointment Time
- Booking Lead Day
- Previous Appointments
- Previous No Shows
- Reminder Sent
- Reminder Channel
- Distance to Clinic
- Waiting Time
- Appointment Status

Appointment outcomes included:

- **Attended**
- **No-Show**
- **Cancelled**

Reminder channels included:

- SMS
- WhatsApp
- Email
- None

The original dataset was preserved while analysis was carried out using working copies.

# Tools & Technologies

### Power BI
Used for:

- Data modelling
- KPI development
- Interactive dashboards
- Segment analysis
- Data visualization
- Testing and validation

### Power Query
Used for:

- Data preparation
- Data cleaning
- Date/date-time handling
- Transformation of analytical fields
- Preparing data for Power BI analysis

### DAX
Used for:

- KPI calculations
- No-show measures
- Reminder-related measures
- Segment-level calculations
- Analytical validation

# 📈 Final KPIs

The final analytics work consolidated four key performance indicators:

No-Show Rate = **48.5%** 
Cancellation Rate = **5.3%** 
Reminder Coverage = **72.7%** 
Average Waiting Time = **24.19 minutes** 

These KPIs provided a high-level view of appointment attendance, cancellations, reminder coverage and operational waiting time.

# Key Analytical Findings

## 1. Previous No-Show History

One of the most important validated findings was the relationship between previous no-show history and observed no-show rates.

There was a total of 2,423 no shows out of 5,000 total appointments **48.5%** 

The analysis showed an increasing observed no-show rate across the previous no-show groups.

This suggests that previous attendance behaviour may be an important factor to consider when developing attendance-support strategies.

However, this is an **observed association and does not establish causation**.

## 2. Distance to Clinic

The analysis also identified a higher observed no-show rate among appointments in the **21+ km** distance group.

This suggests that distance may represent a potential accessibility or travel-related factor worth further investigation.

The finding should not be interpreted as proof that distance directly causes missed appointments.

## 3. Reminder Status

Appointments without a recorded reminder showed a higher observed no-show rate than appointments with a reminder.

Reminder coverage across the dataset was approximately **72.7%**.

This highlighted reminder coverage as an area that could be explored further through targeted operational testing.

The analysis does not establish that reminders alone caused the difference in attendance outcomes.

## 4. Appointment Type

Follow-up appointments recorded the highest observed no-show rate among the appointment types examined during the advanced analysis.

This suggests that follow-up appointments may be a useful segment for additional attendance-support investigation.

# Testing & Validation

Week 7 focused on testing and refinement of the Week 6 analytics outputs.

The objective was not simply to create additional visuals, but to determine whether important analytical results were consistent with the underlying data.

### Testing activities included:

- Reviewing KPI calculations.
- Checking no-show calculations by relevant groups.
- Comparing calculated rates with underlying appointment and no-show counts.
- Testing dashboard calculations and filters.
- Reviewing selected analytical findings against the dataset.
- Checking for unexpected or inconsistent results.
- Documenting validation evidence.
- Retesting after validation.

### Main validated result

The **No-Show Rate by Previous No-Show Group** was tested against the underlying counts.

The expected and actual results matched:

- 0 previous no-shows → **43.5%**
- 1–2 previous no-shows → **54.8%**
- 3+ previous no-shows → **68.8%**

The test was recorded as **PASS**, and no numerical correction was required.

The major refinement was therefore the strengthening of validation evidence and documentation.

# Cross-Track Collaboration

A key part of the final HealthConnect solution was connecting the Data Analytics contribution with other project tracks.

## Data Analytics <> Project Management

Data Analytics provided:

- No-show analysis
- KPI evidence
- Validation results
- Testing evidence

The information supported Project Management's testing documentation, evidence-based status tracking and project coordination.

The validated No-Show Rate by Previous No-Show Group became a documented cross-track testing activity.

## Data Analytics <> Data Science

Data Analytics also shared relevant analytical patterns with the Data Science track.

These included patterns involving:

- Booking lead time
- Previous no-show history
- Appointment type and reminder channel

The Data Science track proposed potential predictive features based on these analytical patterns, including:

- `high_lead_time_flag`
- `chronic_no_show_flag`
- An interaction between `appointment_type` and `reminder_channel`

This created a connection between the descriptive/diagnostic analytics work and the predictive component of the wider solution.

The Data Science analysis was kept distinct from the validated Week 7 analytics figures where differences in grouping or processing existed. This avoided presenting separate analytical outputs as though they were identical.

# How the Tracks Connect

The wider HealthConnect solution brings together several workstreams:

**Data Analytics**  
→ Identifies patterns, measures outcomes and provides evidence.

**Data Science**  
→ Uses relevant analytical patterns to inform potential predictive modelling.

**ML Engineering**  
→ Supports the technical workflow required to operationalize technical components.

**GenAI**  
→ Supports potential patient or administrative interaction.

**Project Management**  
→ Coordinates dependencies, risks, evidence, timelines and final delivery.

The Data Analytics contribution therefore serves as an important **evidence layer** within the wider solution.

# Business Insights & Recommendations

Based on the analytical findings, several areas were identified for further investigation:

### Previous no-show history
Patients with previous no-shows showed higher observed no-show rates.

**Potential action:**  
Consider targeted confirmation or attendance-support workflows for patients with previous no-show history.

### Distance
The 21+ km group showed an elevated observed no-show rate.

**Potential action:**  
Investigate whether accessibility, travel or scheduling barriers are contributing to missed appointments.

### Reminder coverage
Appointments without a recorded reminder showed a higher observed no-show rate.

**Potential action:**  
Explore broader reminder coverage and test whether different reminder approaches perform differently across appointment segments.

### Appointment type
Follow-up appointments showed the highest observed no-show rate among appointment types.

**Potential action:**  
Consider additional confirmation or engagement strategies for follow-up appointments.

These recommendations are **evidence-informed rather than causal conclusions** and should be tested operationally before effectiveness is assumed.

# Analytical Limitations

Several limitations were considered throughout the project:

- The analysis identifies associations rather than proving causation.
- Some high previous-no-show groups contain relatively few records.
- Some dataset variables contain missing values.
- Booking lead-time data required additional quality consideration before being treated as a fully validated predictive feature.
- Different analytical outputs from Data Analytics and Data Science were not silently combined where processing/grouping differed.
- The analytics validation was component-level.
- Complete end-to-end project validation depends on evidence from the wider HealthConnect workstreams.
- Recommendations require real-world testing before their effectiveness can be established.

# Final Week 8 Deliverables

The final Data Analytics submission includes:

### 1. Final Power BI Dashboard

The final dashboard consolidates the analytical work completed throughout the project, including:

- Executive Appointment Overview
- No-Show Drivers
- Patient Support & Appointment Operations
- Advanced No-Show Analysis
- Reminder & Risk Segmentation

### 2. Final Analytics & Decision Support Report

Documents:

- Final KPIs
- Validated findings
- Testing and validation
- Business insights
- Recommendations
- Cross-track contribution
- Limitations
- Final analytics contribution

### 3. Week 8 Project Summary

Provides a concise overview of:

- Planned work
- Completed work
- Validated findings
- Cross-track collaboration
- Changes and improvements
- Final contribution
- Remaining limitations

### 4. Final Presentation

The final presentation communicates:

- The HealthConnect problem
- Data Analytics contribution
- Key findings
- Testing and refinement
- Cross-track collaboration
- Overall HealthConnect solution
- Business value
- Limitations
- Final contribution

### 5. Individual Video Presentation

A recorded presentation explaining the Data Analytics contribution, testing/refinement, cross-track collaboration and role within the wider HealthConnect solution.

### 6. Collaboration Evidence

Supporting evidence documenting Data Analytics collaboration with other project tracks, including Data Science and Project Management.

# Final Outcome

By the end of Week 8, the Data Analytics contribution had progressed from initial data exploration and dashboard development to a more complete evidence-based decision-support package.

The final work demonstrates the progression:

**Data → Analysis → Visualization → Findings → Validation → Business Insights → Recommendations → Cross-Track Integration**

The most important outcome was not simply producing a dashboard, but developing an analytical contribution that could be tested, communicated and connected to the wider HealthConnect solution.

# Internship Learning

The HealthConnect project also represented an important part of my development during the Analyst Lab Africa internship.

Through the project, I strengthened my practical experience in:

- Data analysis
- Data cleaning and preparation
- Power BI
- Power Query
- DAX
- KPI development
- Dashboard design
- Analytical validation
- Business-focused interpretation
- Data storytelling
- Documentation
- Cross-track collaboration
- Communicating technical findings to a wider project team

The project reinforced the importance of moving beyond simply asking:

> **“What does the data show?”**

and also asking:

> **“How reliable is this finding, what does it mean for the business, and how can it support a responsible decision?”**

# Final Internship Week

Week 8 marks the **final week of my Analyst Lab Africa internship** and the completion of my Data Analytics contribution to the HealthConnect Clinic Experience Lab.

This internship provided an opportunity to move from learning analytical concepts to applying them in a structured, project-based environment.

The HealthConnect project served as a practical demonstration of the complete analytical process — from working with raw data to producing insights, validating results, communicating findings and contributing to a multidisciplinary solution.

## Created By: **Chidiebere Lilian Ebulue**

## AnalystLab Africa
