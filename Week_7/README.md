# HealthConnect Clinic - Week 7 Analytics Testing & Refinement

## Project Overview

HealthConnect Clinic is an appointment-based healthcare service project focused on understanding missed appointments and improving the patient support experience.

The core project question is:

> **How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?**

Week 7 focused on **Testing → Refinement → End-to-End Validation**. Building on the Week 6 advanced analytics work, this phase reviewed analytical outputs, validated key calculations and findings against the underlying dataset, documented cross-track testing, and identified remaining dependencies before final integration.

## Week 7 Objectives

The main objectives for the Data Analytics track were to:

- Validate key KPI calculations and analytical findings.
- Test dashboard calculations and filtering behaviour.
- Check analytical findings against the underlying appointment data.
- Test important findings across relevant patient and appointment segments.
- Identify inconsistencies or weaknesses in the analysis.
- Refine unclear or unnecessary analytical outputs where required.
- Document testing evidence and validation results.
- Contribute validated findings to the wider HealthConnect project.
- Support cross-track collaboration with Project Management.
- Prepare the analytics work for Week 8 final integration.

## Week 6 → Week 7 Transition

Week 6 introduced advanced analysis of appointment no-shows, including relationships between previous no-show history, reminder status, appointment characteristics, and patient characteristics.

The main Week 6 analytical outputs included:

- Advanced no-show analysis.
- Reminder and risk segmentation.
- Additional DAX measures.
- Refined Power BI dashboard pages.
- Evidence-based business insights and recommendations.

Week 7 therefore focused on **testing and validating these outputs rather than introducing a completely new analysis**.

The main testing priority was to verify that the observed no-show patterns were correctly calculated and supported by the underlying data.

## Dataset

The project uses the anonymized/fictitious:

**HealthConnect Appointment Dataset**

The dataset contains **5,000 appointment records** and includes variables covering:

- Patient information
- Appointment information
- Booking information
- Previous appointment history
- Previous no-shows
- Reminder status and channel
- Distance to clinic
- Waiting time
- Appointment outcome

### Key appointment outcomes

- Attended
- No-Show
- Cancelled

## Week 7 Testing Approach

Testing was carried out primarily in Power BI using temporary validation tables.

The validation tables compared:

- Total Appointments
- No-Show Appointments
- No-Show Rate

These outputs were compared with the expected Week 6 analytical results.

The approach followed the principle:

> **Test → Finding → Action → Retest → Validated Improvement**

This ensured that findings were based on the underlying data rather than assumptions.

## KPI & Analytical Validation

The main cross-track validation focused on:

### No-Show Rate by Previous No-Show Group

The validation grouped patients according to their previous no-show history and the calculated values matched the expected analytical results.

**Validation result: PASS**

No numerical correction was required.

## Additional Analytical Testing

Additional internal Data Analytics checks were carried out on important Week 6 findings, including:

### Distance to Clinic

The analysis reviewed no-show rates across distance groups, including the 21+ KM group.

The 21+ KM group had an observed no-show rate of approximately **57.8%**.

### Reminder Status

Reminder and no-reminder appointment outcomes were also reviewed.

Observed no-show rates were approximately:

- **Reminder:** 47.4%
- **No Reminder:** 51.4%

These results were used as analytical evidence rather than proof of causation.

## Dashboard Testing

The Power BI dashboard was reviewed to ensure that:

- KPI calculations were consistent with the underlying data.
- Grouped no-show rates matched the source calculations.
- Dashboard filters produced appropriate changes in displayed results.
- Analytical visuals remained consistent with the validated findings.
- The dashboard supported interpretation of the tested findings.

The testing process did not identify a numerical calculation error requiring correction.

## Refinement

The main Week 7 refinement was **evidence and validation documentation rather than numerical correction**.

The analytical work was strengthened by:

- Documenting the validation process.
- Recording the expected and actual results.
- Separating verified findings from unverified assumptions.
- Documenting the Data Analytics → Project Management testing activity.
- Maintaining evidence-based testing statuses.
- Clarifying the limitations of component-level validation.

The updated Power BI file included the analytical work and supporting validation calculations used during testing.

## Cross-Track Collaboration

### Data Analytics → Project Management

The primary verified cross-track testing activity was conducted between the **Data Analytics** and **Project Management** tracks.

### Dependency

The Week 6 finding relating previous no-show history to future no-show outcomes required validation before being carried forward into the wider project.

### Component Tested

**No-Show Rate by Previous No-Show Group**

### Information Provided by Data Analytics

Data Analytics provided:

- The underlying validation output.
- Expected grouped no-show rates.
- Appointment and no-show counts.
- Evidence supporting the analytical finding.

### Information Received from Project Management

Project Management used the validation evidence to:

- Record the testing activity.
- Update the project testing/validation documentation.
- Confirm the status of the tested component.
- Track remaining cross-track dependencies.

### Testing Outcome

The expected and actual values were consistent.

**Result: PASS**

No corrective calculation was required.

## Validated Finding

The Week 7 testing confirmed that the observed relationship between previous no-show history and current no-show rate was reproduced in the underlying data:

- Patients with no previous no-shows: **43.5%**
- Patients with 1–2 previous no-shows: **54.8%**
- Patients with 3+ previous no-shows: **68.8%**

This finding can therefore be carried forward as a **validated analytical finding**.

However, the analysis describes an observed association and does not establish that previous no-shows directly cause future no-shows.

## Key Findings & Outcomes

The Week 7 testing produced the following outcomes:

1. The overall observed no-show rate remained **48.5%**.
2. The previous no-show history finding was successfully validated.
3. No calculation inconsistency was identified in the main cross-track test.
4. Additional internal checks were performed for distance and reminder status.
5. No numerical correction was required.
6. The testing evidence was formally documented.
7. The validated finding was retained for wider project integration.
8. Full end-to-end validation remained dependent on evidence from the other project tracks.

## Recommendations

Based on the validated analytical findings, the project can consider:

- Using previous no-show history as a potential feature for future risk segmentation or modelling.
- Considering reminder status and distance to clinic as additional analytical inputs.
- Exploring targeted patient-support interventions for groups with higher observed no-show rates.
- Continuing to validate these patterns as additional modelling and AI components are developed.
- Avoiding causal interpretation of the current observational findings without further testing.

## Limitations

The Week 7 analytics validation has several limitations:

- The validation was primarily conducted at the component level.
- The dataset is an anonymized/fictitious project dataset.
- Observed relationships do not establish causation.
- Some high previous-no-show groups contain relatively few records.
- Full end-to-end solution validation was not completed within the Data Analytics track.
- The validated analytics findings therefore represent one component of the wider HealthConnect solution.

## Week 7 Outcome

The Data Analytics component completed its main testing activity successfully.

The most important validated output was the **No-Show Rate by Previous No-Show Group**, which was independently checked against the underlying appointment counts and reproduced the expected results.

The main improvement during this phase was stronger documentation and evidence control rather than a change to the numerical analytical results.

## Week 8 Transition

Week 8 focuses on:

- Final integration of the project outputs.
- Carrying validated Data Analytics findings into the wider solution.
- Closing outstanding cross-track dependencies.
- Finalizing project documentation.
- Preparing the final project presentation.

The Data Analytics track will carry forward the validated findings and supporting evidence while remaining aligned with the outputs and requirements of the other project tracks.

## Project Files

This repository contains the main Week 7 deliverables:

### `HealthConnect_Analytics_Testing_and_Refinement_Report.pdf`

Detailed Data Analytics report covering:

- Week 6 → Week 7 transition
- Testing approach
- KPI validation
- Analytical validation
- Dashboard testing
- Refinement
- Cross-track testing
- Validated findings
- Recommendations
- Limitations
- Week 8 recommendations

### `HealthConnect_Clinic_Project_Summary_Report.pdf`

Brief project summary covering:

- What was planned
- What was completed
- What was tested
- What was improved
- What was validated
- Cross-track collaboration
- Information exchanged
- What changed
- Findings/outcomes
- Challenges
- Decisions
- Remaining issues
- Contribution
- Week 8 focus

### `HealthConnect_Advanced_Analytics.pbix`

Updated Power BI project file containing the HealthConnect analytics dashboard and supporting Week 7 validation work.

The Power BI file demonstrates the analytical outputs, dashboard development, calculations, and validation tables used during the testing phase.

## Tools Used

- **Microsoft Power BI**
- **Microsoft Word**.

## Created By

**Chidiebere Lilian Ebulue**

## AnalystLab Africa
