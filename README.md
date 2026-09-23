# HealthConnect-Lab
For Week 4 on the AnalystLab Africa Internship, I'm looking at HealthConnect data. . The goal for the project is to understand which factors are associated with patients missing scheduled appointments, quantify the operational impact, and produce data-driven insights and KPIs that clinic staff can use to identify high-risk appointments and inform intervention decisions.

# Week 5 Project Continuation
For Week 5, I delved into the HealthConnect data, examining appointment no-shows and cancellations for a healthcare provider, using 5,000 appointment records to identify the strongest factors associated with missed appointments and produce actionable KPIs and dashboards for clinic operations.

## Problem
Missed appointments (no-shows) cost clinics wasted capacity, staff time, and delayed care for other patients. This project analyzes appointment-level data to find out how the clinic can use their data to reduce missed appointments and improve patient support experience.

## Key Findings
- No-show rate: 48.46% (2,423 of 5,000 appointments)
- Reminder effectiveness: reminders are associated with a 4.03pp (≈7.85% relative) reduction in no-shows
- Repeat-offender concentration: 40% of patients (679 of 1,696) account for 72.4% of all no-shows — the highest-leverage finding for targeting intervention
- Confirmed prior no-show history remains the strongest associated factor

![Dashboard Preview](./Week%205/preview.jpg)

Used Power BI (Power Query + DAX) for KPI calculation and dashboard visualization.

# Week 6 Progress
- Revised the dashboard from the Week 5 version into a sharper, findings-focused layout (Appointment Outcome, Reminder Status, Distance to Clinic, and Booking Lead Days panels), and scoped the analysis specifically to Attended vs. No-Show comparisons. 

- Week 5's dashboard surfaced factors without interpreting them. Week 6's dashboard was simplified, dropping panels that weren't adding interpretive value in favor of ones that support the four advanced findings.

![Dashboard Preview](./Week%206/V2.jpg)

## More Findings
- Distance shows a measurable separation: Attended patients average 9.67km from the facility versus 10.53km for No-Show patients.
- Booking lead time shows a visible effect. Patients averaging around 34 lead days were more likely to no-show than those around 24 days.

I delivered the first version of findings that moves beyond description into interpretation — giving the project concrete, stakeholder-ready reasoning (e.g., the mobile clinic and booking cut-off recommendations) rather than just metrics.

# Week 7 Progress - Analytical Testing
WStatistically validated all three Week 6 findings using a chi-square test and two t-tests, and corrected a scoping error from Week 6 where Cancelled appointments were excluded from the dashboard, which was skewing the results, and have now been reintroduced.

## Key Findings (as of Week 7)
- No-show rate: 48.46% (2,423 of 5,000 appointments)
- Repeat-offender concentration: 72.43% of no-shows come from patients with 2+ prior no-shows (679 of 1,696 patients)
- Reminder effectiveness: 4.03pp reduction in no-shows — statistically significant (p = 0.00346) but a modest association
- Distance to clinic: 0.86km average gap between No-Show and Attended patients — statistically significant (p = 8.14×10⁻⁶) but a modest influence
- Booking lead time: 10.01-day average gap between No-Show and Attended patients — statistically significant (p = 1.07×10⁻⁹⁰) and the strongest validated driver of the three.

All three relationships are confirmed statistically real, not artifacts of sample size or chance. Booking lead time is by far the most decisive and actionable of the three.

# Week 8 - Finalizing
My final component is The HealthConnect Analytics & Decision Support Package consisting of validated KPIs, dashboard, and business recommendations. It addresses the problem of identifying and statistically confirming which factors drive appointment no-shows, so HealthConnect can prioritize interventions with confidence. It is currently validated and ready for final packaging to handover back to the facility for action. 

![Final Dashboard](./Week%208/w8.jpg)
