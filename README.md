# HR_Employee-Enagagement-Attrition-Analytics-Project
A real world analytics project examining a global organization HR data. Utilizing a suite of analytical methods such as descriptive analysis, driver analysis, predictive modelling, segmentation and clustering.

## Disclaimer
This project was developed using company‑sponsored data as part of an academic module.  
Due to confidentiality policies, the original dataset cannot be shared publicly.  
All sensitive information has been anonymized, generalized, or redacted to prevent traceability.  
The repository showcases the analytical methods, workflows, and deliverables, but does not expose proprietary or confidential company data.

## Data Privacy Note
To comply with organizational data governance standards:
- **Anonymization:** Employee identifiers and personal attributes were anonymized to remove direct links to individuals.  
- **Redaction:** Sensitive company names, logos, and proprietary metrics were removed or replaced with generalized placeholders.  
- **Schema Sharing:** Only the anonymized schema and data dictionary are provided to illustrate structure without revealing raw values.  
- **Controlled Outputs:** Dashboards, reports, and slides are included with sensitive elements blurred or redacted, ensuring insights are shared responsibly.  

This approach demonstrates the ability to apply analytics methods in a real‑world context while maintaining strict adherence to confidentiality and ethical data handling practices.

## Overview
This project examines how engagement influences voluntary attrition by analysing two engagement surveys held in two seperate time event. The 2024 survey establishes a baseline engagement attrition relationship, while the 2026 survey reflects the organisation's current state following substantial employee turnover.

## Business Problem
The organisation faces a high attrition rate that poses a material risk to a consultancy driven business exceptionally where expertise is the primary value driver. Simultaneously, employee engagement levels are declining especially in the critical employee segment of High performers and Senior Leadership. Attrition within these segments poses specific risks to leadership continuity, capability retention, and overall business performance.
The business question is thus, “How can the organisation identify flight risk employees, uncover key areas of employee engagement drivers, and take targeted actions to improve retention and mitigate attrition?”

## Business Objectives
- Reduce voluntary attrition among critical talent segments.
- Improve retention of high performers and employees in key roles.
- Increase overall engagement levels through targeted, data-driven interventions.
- Provide leadership with a clear understanding of key engagement and attrition drivers.
- Enable proactive identification of flight-risk employees through a predictive framework.
- Equip HR business partners with interactive dashboards and actionable insights to support decision making.

## Technical Approach & Deliverables

| Objectives | What It Does | Business Value |
| --- | --- | --- |
| Build an Integrated Analytical Dataset | Clean, integrate and structure HR data from multiple sources into a relational model (3NF) to produce ready dataset. | Establishes realiable, auditable data foundation that underpinsall downstream analysis and decisions. |
| Identify & validate Engagement Drivers | Conduct exploratory data analysis, hypothesis testing (t-tests, chi-square) and effect size analysis. | Moves te organization form intuition to evidence. |
| Analyse the Engagement–Attrition Relationship | Link 2024 engagement drivers to actual attrition outcomes (Oct 2024 – Feb 2026) to test whether engagement is a leading indicator of attrition risk. | Validates engagement as a predictive metric, strengthening the case for early intervention. |
| Develop a predictive Model (decision tree) | Build an interpretable classification model to identify flight-risk employees and extract transparent decision rules. | Enables proactive, individual level retention action while maintaining explainability for HR and leadership. |
| Segment Employees into Risk Profiles | Cluster employess into actionable groups such as high performer-at-risk, long-tenure-declining, and new-joiner cohorts. | Supports differentiated retention strategies tailored to each segment;s drivers and risk profile. |
| Deliver Dashboard & Actionable Insights | Develop a Power BI dashboard that integrates driver, segment, and risk analyses into interactive decision tool. | Equips HR and leadership with a live, evidence bases platform to guide retention decisions and track progress. |

## Tools & Methods
- **Excel:** Data loading, cleaning and EDA
- **Power BI:** Dashboard creation and visualization, Data modelling (schema)
- **Orange:** Decision Tree Modeling (Chi-Sqaure test), Cluster Analysis
- **MS word:** for project report
- **MS Powerpoint:** for presentation

## Dataset
- **Dataset not shared due to confidentiality**
- Description: Organization sourced HR dataset containing 18,000 employee record (54 Columns). An integrated dataset containing employee demographic, logged survey response and questions across 2024 and 2026, and organization information.
- Data Preparation performed in excel:
  - Data cleaning of column heterogeneity
  - Data anonymization of employee details
  - Binning of columns Tenure, Age Group, Performance Rating 
  - Impute missing values with median values
  - New column computation for defined "Critical Talent Leaver"
- Data Transformation: normalization performed in Power BI to achieve Third Normal Form (3NF)
  <img width="2617" height="1379" alt="image" src="https://github.com/user-attachments/assets/8e699ae5-a706-4854-a50c-4bc516d03d88" />
- Data Dictionary
  <img width="1507" height="507" alt="image" src="https://github.com/user-attachments/assets/85888080-f653-47b5-b795-da699c98e7db" />
  <img width="1625" height="393" alt="image" src="https://github.com/user-attachments/assets/915d14cf-80fc-4df9-bbe6-7f1b7bc77417" />
  <img width="1602" height="477" alt="image" src="https://github.com/user-attachments/assets/b808cbbb-c5c9-454a-8219-1ef57f53299e" />
  <img width="1487" height="328" alt="image" src="https://github.com/user-attachments/assets/e951ac16-ccfe-4b3c-91ad-dd749928cb59" />
  <img width="1518" height="232" alt="image" src="https://github.com/user-attachments/assets/654dc2ee-cfdf-42aa-ae4f-e5ed58d48ed1" />

## Analytical Methods and Results
The hypothesis was that vountary leavers had statistically lower engagement than stayers. Two formal test applied to validate this.
**Result:** Both T-test and Chi-square test rejected both null hypothesis therefore proving that mean score of both cohorts (voluntary & non-voluntary leavers) are equal and attrition outcome is dependant on engagement level.
1. **Hypothesis Testing**
   - T-Test (independent two-sample, two tail): Compared mean engaement score for stayers (n=9,086) vs voluntary leavers (n=1,765). Returned with p-value below 0.001.
     <img width="720" height="263" alt="image" src="https://github.com/user-attachments/assets/d13344d2-5f02-415a-84fb-04566558513d" />
   -Chi-Square Test of Independence: Tested whether engagement level is independent of attrition outcome. Returned with p-value below 0001.
     <img width="726" height="138" alt="image" src="https://github.com/user-attachments/assets/baba4f63-a3d7-4921-99ca-34a3a0392565" />

##



