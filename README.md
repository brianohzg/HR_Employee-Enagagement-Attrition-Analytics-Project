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

###Technical Approach & Deliverables

| Objectives | What It Does | Business Value |
| --- | --- | --- |
| Build an Integrated Analytical Dataset | Clean, integrate and structure HR data from multiple sources into a relational model (3NF) to produce ready dataset. | Establishes realiable, auditable data foundation that underpinsall downstream analysis and decisions. |
| Identify & validate Engagement Drivers | Conduct exploratory data analysis, hypothesis testing (t-tests, chi-square) and effect size analysis. | Moves te organization form intuition to evidence. |
| Analyse the Engagement–Attrition Relationship | Link 2024 engagement drivers to actual attrition outcomes (Oct 2024 – Feb 2026) to test whether engagement is a leading indicator of attrition risk. | Validates engagement as a predictive metric, strengthening the case for early intervention. |
| Develop a predictive Model (decision tree) | Build an interpretable classification model to identify flight-risk employees and extract transparent decision rules. | Enables proactive, individual level retention action while maintaining explainability for HR and leadership. |
| Segment Employees into Risk Profiles | Cluster employess into actionable groups such as high performer-at-risk, long-tenure-declining, and new-joiner cohorts. | Supports differentiated retention strategies tailored to each segment;s drivers and risk profile. |
| Deliver Dashboard & Actionable Insights | Develop a Power BI dashboard that integrates driver, segment, and risk analyses into interactive decision tool. | Equips HR and leadership with a live, evidence bases platform to guide retention decisions and track progress. |

##Dataset
- Description: Organization HR dataset containing 18,000 employee record (54 Columns). An integrated dataset containing employee demographic, logged survey response and questions across 2024 and 2026, and organization information.
- 
