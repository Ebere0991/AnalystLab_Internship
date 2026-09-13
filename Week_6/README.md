# HealthConnect Clinic — Week 6: Advanced Analytics & Decision Support

## Project Overview

This repository contains my **Week 6 Data Analytics deliverables** for the HealthConnect Clinic project, developed as part of the AnalystLab Africa internship.

The HealthConnect project focuses on one central question:

**How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?**

Week 6 builds directly on the Week 5 appointment attendance and no-show analysis.

While Week 5 focused primarily on understanding the dataset, identifying patterns, developing initial KPIs, and building the first Power BI dashboard, Week 6 moved into **advanced analysis, validation, segmentation, decision support, and cross-track integration**.

The goal was to investigate important findings more deeply, determine whether the observed patterns remained meaningful across different patient and appointment segments, refine the analytical conclusions, and translate the findings into actions that could support Week 7 testing and refinement.

# Week 6 Objectives

The main objectives for Week 6 were to:

- Investigate important findings identified during Week 5.
- Perform deeper analysis across patient, appointment, and operational segments.
- Examine relationships between key factors associated with missed appointments.
- Validate important Week 5 KPIs and findings.
- Refine the interpretation of no-show patterns.
- Identify high-impact risk segments.
- Translate analytical findings into practical business recommendations.
- Improve the Power BI dashboard with advanced analytical views.
- Provide relevant findings for downstream project planning and testing.
- Complete meaningful cross-track collaboration.
- Define analytical requirements and priorities for Week 7 testing and refinement.
- Document limitations and areas requiring further investigation.

# Week 5 → Week 6 Transition

Week 5 established the analytical foundation for the HealthConnect project.

The initial analysis identified several areas requiring deeper investigation, including:

- High overall no-show rates.
- The relationship between previous no-show history and future attendance.
- Higher observed no-show rates among patients living farther from the clinic.
- Differences between appointments with and without reminders.
- Differences in attendance patterns across appointment types.
- Reminder coverage across appointment categories.

Week 6 therefore moved from:

**"What is happening?"**

to:

**"Do these patterns remain meaningful when we examine them across multiple factors, and how can HealthConnect use the findings?"**

The Week 6 analysis retained the Week 5 dataset and analytical foundation while introducing additional segmentation and cross-variable analysis.

# Advanced Analysis

## 1. Previous No-Show History

Previous no-show history was investigated as an important potential indicator of future missed appointments.

Patients were grouped into:

- `0` previous no-shows
- `1–2` previous no-shows
- `3+` previous no-shows

This grouping was introduced to make the analysis more robust and reduce overinterpretation of very small individual groups.

The Week 6 analysis showed an increasing observed no-show rate.

The pattern observed indicated that previous attendance behaviour is an important risk signal for future missed appointments.

However, the relationship should be interpreted as an **association rather than proof of causation**.

# 2. Appointment Type and Previous No-Show History

The analysis examined whether previous no-show history remained associated with attendance when appointment type was considered.

A matrix was developed comparing:

- Appointment Type
- Previous No-Show Group
- No-Show Rate

This provided a more detailed view than the Week 5 appointment-type analysis alone.

The analysis showed that no-show rates generally increased as previous no-show history increased across appointment types.

This supports the use of previous attendance behaviour as a potential risk segmentation variable.

# 3. Distance and Previous No-Show History

Distance from the clinic was investigated together with previous no-show history.

The analysis examined:

- Distance Group
- Previous No-Show Group
- No-Show Rate

The results showed that both distance and previous no-show history can be useful for identifying higher-risk appointment segments.

The `21+ km` distance group recorded a higher overall observed no-show rate than the shorter-distance groups.

However, distance should not be interpreted as a direct cause of missed appointments because other accessibility, scheduling, transport, socioeconomic, and patient-related factors were not available in the dataset.

# 4. Distance and Reminder Status

Week 6 also examined the relationship between:

- Distance Group
- Reminder Status
- No-Show Rate

This analysis was designed to determine whether the reminder-related pattern observed in Week 5 remained visible across different distance segments.

The resulting visualization allows HealthConnect to identify whether reminder coverage appears to be associated with lower observed no-show rates within different distance groups.

Again, these results represent observed associations and should be validated through controlled testing before being treated as evidence of causal impact.

# 5. Reminder and Risk Segmentation

Reminder effectiveness was investigated beyond the simple Week 5 comparison of reminder channels.

Week 6 examined reminder performance across:

- Appointment Type
- Reminder Channel
- Reminder Status
- Appointment Time
- Distance Group

The dashboard includes comparisons between reminder coverage and observed no-show rates across appointment types.

This provides a more useful decision-support view than looking at reminder coverage alone.

# 6. Appointment Type and Reminder Channel

A matrix was created to compare:

- Appointment Type
- Reminder Channel
- No-Show Rate

This allows differences in observed no-show rates to be examined across combinations of appointment type and reminder channel.

The analysis supports further testing of whether reminder strategies should be differentiated according to appointment characteristics rather than applying a single reminder approach to all patients.

# 7. Appointment Time and Reminder Status

Week 6 also examined no-show rates across:

- Morning
- Afternoon
- Evening

while comparing:

- No Reminder
- Reminder

This provides additional segmentation for future testing and allows HealthConnect to investigate whether reminder strategies perform differently across appointment time periods.

# KPI Validation and Refinement

The Week 6 dashboard retained and validated the core Week 5 KPIs.

The refined dashboard includes:

No-Show Rate - 48.5% 
Cancellation Rate - 5.3% 
Reminder Coverage Rate - 72.7% 
Average Waiting Time - 24.19 minutes 

Additional Week 6 analytical measures included:

- No-Reminder No-Show Rate
- Reminder No-Show Rate
- Reminder No-Show Gap
- Repeat No-Show Rate

These additional measures were introduced to support deeper analysis rather than simply repeating the Week 5 dashboard.

# Power BI Dashboard

The Week 6 Power BI dashboard was developed as an extension of the Week 5 analytical work.

The Week 5 dashboard was retained as the baseline, while new analytical pages were added for Week 6.

## Dashboard Page 4 — Advanced No-Show Analysis

This page investigates the interaction between previous attendance behaviour and other appointment characteristics.

### Key visualizations include:

- No-Show Rate by Previous No-Show History
- No-Show Rate by Age Group and Previous No-Show History
- No-Show Rate by Distance Group and Reminder Status
- No-Show Rate by Appointment Type and Previous No-Show History
- No-Show Rate by Distance Group and Previous No-Show History

### Purpose

The page investigates whether important Week 5 patterns remain consistent when multiple factors are examined together.

# Dashboard Page 5 — Reminder and Risk Segmentation

This page focuses on reminder coverage and potential risk segments.

### Key visualizations include:

- Reminder Coverage by Distance Group
- No-Show Rate by Appointment Type and Reminder Status
- Reminder Coverage Rate and No-Show Rate by Appointment Type
- No-Show Rate by Appointment Time and Reminder Status
- No-Show Rate by Appointment Type and Reminder Channel

### Purpose

The page provides a deeper view of reminder coverage and supports future testing of targeted reminder strategies.

# Business Insights

The Week 6 analysis produced several important insights.

### 1. Previous no-show behaviour is an important risk signal

Observed no-show rates increased from:

**43.5% → 54.8% → 68.8%**

as previous no-show history increased from `0` to `1–2` and then `3+`.

This suggests that previous attendance behaviour could be useful for identifying appointments that may require additional engagement.

### 2. Distance remains a relevant segmentation factor

Patients in the `21+ km` distance group recorded a higher observed no-show rate than shorter-distance groups.

This suggests that distance-related barriers may warrant additional investigation.

Possible factors could include transportation, accessibility, travel time, appointment scheduling, or other constraints.

### 3. Reminder coverage represents an opportunity for further testing

Appointments without reminders showed a higher observed no-show rate than appointments that received reminders.

However, reminder assignment may be influenced by other factors, so the observed relationship should not be interpreted as proof that reminders directly caused the difference.

This makes reminder strategy an important candidate for controlled Week 7 testing.

### 4. Appointment type shows some differences, but appears less influential than previous attendance behaviour

Appointment types displayed differences in observed no-show rates, but the deeper analysis indicates that previous no-show history provides a stronger segmentation signal.

This suggests that HealthConnect should avoid relying on appointment type alone when identifying higher-risk appointments.

# Recommendations

Based on the Week 6 analysis, the following actions are recommended for further testing and validation.

## 1. Test enhanced reminders for patients with previous no-show history

Patients with previous missed appointments should be considered for targeted reminder or follow-up strategies.

Possible approaches could include:

- Earlier reminders
- Multiple reminder touchpoints
- Confirmation requests
- Follow-up communication for higher-risk patients

These approaches should be tested before being implemented as permanent policy.

## 2. Investigate distance-related attendance barriers

HealthConnect should investigate why patients living farther from the clinic have higher observed no-show rates.

Potential areas for investigation include:

- Transportation difficulties
- Travel time
- Appointment scheduling
- Accessibility
- Rescheduling options

## 3. Evaluate reminder strategy by appointment segment

Rather than assuming that one reminder approach works equally for all patients, Week 7 testing should examine reminder performance across:

- Appointment type
- Appointment time
- Distance group
- Previous no-show history

## 4. Use previous attendance behaviour as a potential risk feature

Previous no-show history may be useful as a candidate feature for downstream predictive analytics or risk segmentation.

However, this should be evaluated alongside other relevant features rather than used as a standalone decision rule.

## 5. Validate findings through controlled testing

The Week 6 analysis identifies associations.

Week 7 should therefore focus on testing whether targeted interventions actually improve attendance.

# Week 7 Testing Requirements

The Week 6 analysis identified the following priorities for Week 7.

### 1 — Enhanced reminder strategy

Test whether enhanced reminder strategies improve attendance among patients with previous no-show history.

### 2 — Distance-related support

Test or investigate targeted support for patients living farther from the clinic.

### 3 — Reminder coverage and channel performance

Evaluate reminder coverage and channel performance across appointment types and other relevant segments.

### 4 — Higher-risk appointment segments

Monitor attendance among patients identified through combinations of risk factors such as:

- Previous no-show history
- Distance
- Reminder status
- Appointment characteristics

### 5 — Validate observed patterns

Determine whether the Week 6 risk patterns remain consistent during testing.

# Cross-Track Integration — Project Management

A key Week 6 requirement was meaningful cross-track collaboration.

During Week 6, the Data Analytics track collaborated with the **Project Management workstream**.

The collaboration was not treated as communication alone. An actual analytical output was exchanged and used to inform project coordination.

## What Project Management Provided

The Project Management workstream provided:

- Project integration context
- Workstream dependencies
- Current priorities
- Risk and issue considerations
- Integration requirements
- Week 7 testing and refinement focus
- Coordination requirements
- Readiness considerations
  
### Data Analytics → Project Management

Analytical findings and remaining analytical requirements were provided to PM.

### Project Management → Data Analytics

PM provided project priorities, integration context, dependencies, and Week 7 testing/refinement requirements.

## What Changed as a Result

The analytical findings were incorporated into the PM integration and dependency view.

The exchange helped identify:

- Previous no-show history as an important analytical consideration
- Booking lead time as an area requiring analytical attention
- Remaining analytical work
- Testing requirements for Week 7
- Dependencies that require monitoring before broader testing

The collaboration also helped distinguish between:

**Completed integration**

and

**technical workstreams that still require supporting evidence.**

## How the Output Was Used

The Data Analytics output was used by Project Management as an evidence-based input for:

- Integration coordination
- Dependency tracking
- Week 7 testing preparation
- Risk and issue monitoring
- Identification of remaining analytical requirements

# Limitations

Several limitations should be considered when interpreting the Week 6 findings.

### Data limitations

- The dataset contains limited patient and operational variables.
- Distance may represent multiple underlying factors that are not directly measured.
- Reminder assignment may not be random.
- Some fields contain missing values.
- Small subgroups can produce unstable percentages.
- High previous no-show groups should be interpreted cautiously where sample sizes are limited.

### Analytical limitations

- The analysis identifies associations rather than causation.
- The Week 6 dashboard does not establish that reminders directly cause attendance improvement.
- Additional statistical or predictive modelling may be required to validate relationships.
- Multi-variable modelling remains an area for further development.

### Project limitations

- Data Science, ML Engineering, and Generative AI integration readiness could not be confirmed without verified supporting evidence.
- Some downstream technical dependencies remain pending.
- Week 7 testing is required to determine whether the identified intervention opportunities produce measurable improvements.

# Created By:

## **Chidiebere Lilian Ebulue** 

## AnalystLab Internship
