# HR_Employee-Enagagement-Attrition-Analytics-Project
A real world analytics project examining a global organization HR data. Utilizing a suite of analytical methods such as descriptive analysis, driver analysis, predictive modelling, segmentation and clustering.

---

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

---
## Competency Showcase
This project demonstrated:
- **Technical Skills:** Business Statistics, Machine Learning (Decision Tree), Clustering, Data Management, Data Modeling
- **Tools:** Excel, Power BI, Orange, PowerPoint
- **Business Impact:** Industry Insight and organizational recommendation generation, Data storytelling
- ## Note
  Due to simplicity, this README file does not highlight the full exhaustive materials, steps and documents listed in the actual project. Other items, work, skills and topics covered are:
  -    Gantt and Burndown Chart
  -    Work Breakdown Sheet
  -    Project Powerpoint storytelling slides
  -    Full Project Report
  -    Stakeholder Analysis and Requirement Envisiong
  -    Data Risk Register

---

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
| Segment Employees into Risk Pros | Cluster employess into actionable groups such as high performer-at-risk, long-tenure-declining, and new-joiner cohorts. | Supports differentiated retention strategies tailored to each segment;s drivers and risk pro. |
| Deliver Dashboard & Actionable Insights | Develop a Power BI dashboard that integrates driver, segment, and risk analyses into interactive decision tool. | Equips HR and leadership with a live, evidence bases platform to guide retention decisions and track progress. |

## Tools & Methods
- **Excel:** Data loading, cleaning and EDA
- **Power BI:** Dashboard creation and visualization, Data modelling (schema)
- **Orange:** Decision Tree Modeling (Chi-Sqaure test), Cluster Analysis
- **MS word:** for project report
- **MS Powerpoint:** for presentation 

## Dataset
- **Dataset not shared due to confidentiality**
- Description: Organization sourced HR dataset containing 18,000 employee record (54 Columns). An integrated dataset containing employee demographic, logged survey response and questions across 2024 and 2026, and
  organization information.
- Data Preparation performed in excel:
  - Data cleaning of column heterogeneity
  - Data anonymization of employee details
  - Binning of columns Tenure, Age Group, Performance Rating 
  - Impute missing values with median values
  - New column computation for defined "Critical Talent Leaver"
- Data Transformation: normalization performed in Power BI to achieve Third Normal Form (3NF)
  <img width="2000" height="1000" alt="image" src="https://github.com/user-attachments/assets/8e699ae5-a706-4854-a50c-4bc516d03d88" />
- Data Dictionary
  <img width="1507" height="507" alt="image" src="https://github.com/user-attachments/assets/85888080-f653-47b5-b795-da699c98e7db" />
  <img width="1625" height="393" alt="image" src="https://github.com/user-attachments/assets/915d14cf-80fc-4df9-bbe6-7f1b7bc77417" />
  <img width="1602" height="477" alt="image" src="https://github.com/user-attachments/assets/b808cbbb-c5c9-454a-8219-1ef57f53299e" />
  <img width="1487" height="328" alt="image" src="https://github.com/user-attachments/assets/e951ac16-ccfe-4b3c-91ad-dd749928cb59" />
  <img width="1518" height="232" alt="image" src="https://github.com/user-attachments/assets/654dc2ee-cfdf-42aa-ae4f-e5ed58d48ed1" />

## Analytical Methods and Steps
1. **Hypothesis Testing**
The hypothesis was that vountary leavers had statistically lower engagement than stayers. Two formal test applied to validate this.
**Result:** Both T-test and Chi-square test rejected both null hypothesis therefore proving that mean score of both cohorts (voluntary & non-voluntary leavers) are equal and attrition outcome is dependant on engagement level.
   - T-Test (independent two-sample, two tail): Compared mean engaement score for stayers (n=9,086) vs voluntary leavers (n=1,765). Returned with p-value below 0.001.
   - <img width="600" height="230" alt="image" src="https://github.com/user-attachments/assets/d13344d2-5f02-415a-84fb-04566558513d" />

   - Chi-Square Test of Independence: Tested whether engagement level is independent of attrition outcome. Returned with p-value below 0.001.
   - <img width="600" height="110" alt="image" src="https://github.com/user-attachments/assets/baba4f63-a3d7-4921-99ca-34a3a0392565" />

2. **Driver Gap Analysis**
**Variance Chart in Engagement Score**
- Each of the 24 engagement drivers was scored separately for stayers and voluntary leavers, and the gap between the two scores was computed. Voluntary leavers scored lower on every single driver. Note that binning of 24  drivers was deliberatly avoided to retain driver-level granularity to drive precise diagnosis instead of broad plans.
  <img width="700" height="370" alt="image" src="https://github.com/user-attachments/assets/231dc8be-53de-4d02-b571-41e5db98a372" />

3. **Driver Priorities Scatter**
- This analysis was operationalised through an interactive Power BI dashboard, enabling dynamic exploration of attrition drivers. Each driver was plotted on a scatter chart with the stayer engagement score on the X-axis and the leaver–stayer engagement gap on the Y-axis. This visualisation allowed quick identification where gaps are most pronounced relative to baseline engagement levels (Mean). In particular, the bottom-left quadrant, drivers that score low among stayers and exhibit large negative leaver-vs-stayer gaps, represents the highest leverage area for intervention, where targeted action is most likely to improve engagement and reduce voluntary attrition.
  <img width="800" height="430" alt="image" src="https://github.com/user-attachments/assets/5e7360e9-1116-4e67-9f61-640d12214607" />

4. **Decision Tree Modeling**
- File: [Orange_Decision Tree_Model.ows](https://github.com/brianohzg/HR_Employee-Enagagement-Attrition-Analytics-Project/blob/main/Orange_Decision%20Tree_Model.ows)
- A decision tree classifier in Orange was used to predict attrition from 24 engagement drivers. Separate trees were built for the workforce, critical talent, and regions (AEUK, AMECA, ANZ, ASIA) to highlight segment-specific drivers. The interpretable tree was chosen over complex ensembles to provide transparent, HR‑readable decision rules. For simplicity, the focus is on the attrited critical talent segment for modeling. 
  <img width="1100" height="490" alt="image" src="https://github.com/user-attachments/assets/f309097d-bee6-4be4-96d1-5d75b4732e3c" />
  <img width="800" height="390" alt="image" src="https://github.com/user-attachments/assets/517fd2d3-0ea9-4cfc-a168-8f221a93f01e" />

5. **Clustering Analysis**
- File: [Orange_Clustering_Model.ows](https://github.com/brianohzg/HR_Employee-Enagagement-Attrition-Analytics-Project/blob/main/Orange_Clustering_Model.ows)
- A clustering analysis was performed in Orange using engagement, tenure, job grade, performance rating, and demographic attributes as features. Three natural segments emerged. The clusters were profiled by their characteristics and engagement index, and labelled qualitatively as Thriving, Loudly Quitting, and Quietly Quitting.
  <img width="1100" height="420" alt="image" src="https://github.com/user-attachments/assets/58025ab9-43fa-49c1-b437-0cfa90772655" />
  <img width="700" height="420" alt="image" src="https://github.com/user-attachments/assets/78d06dcc-0898-4c0f-bfdf-ea8e23117917" />

## Results & Recommendations
1. **Insights**
   - **Engagement is a Statisically Significaant predictor of voluntary attrition**
     - Stayers had an Engagement Index of 73 in 2024. Involuntary leavers scored higher at 76. Voluntary leavers scored just 67. That is a 6-point gap below stayers and a 9-point gap below involuntary leavers. The T-test and Chi-Square test (Section 9.1) confirm this is not random variation. Higher engagement is consistently and strongly associated with lower voluntary attrition (p < 0.001 in both tests).
   - **Top Engagement Drivers Tied to Attrition**
     - The diverging-bar gap analysis shows that voluntary leavers scored lower than stayers on every one of the 24 engagement drivers. Intent to Stay had the largest gap at 10.5 points but is interpreted as an early-warning signal rather than a causal driver. The next largest gaps are Recognition (-6.9), Company Direction (-5.8), Growth (-5.7), and Well-being (-5.5). Plotted on the scatter chart, the four drivers that fall into the high-impact, low-score quadrant — the prioritisation target — are Recognition, Well-being, Company Direction (with Communication and Transparency), and Growth.
   - **Demographic Specific Drivers from Decision Trees**
     - The decision-tree segmentation guided the regional and talent-specific strategy. The 2026 Engagement Index appears as the top splitting factor in every segment, followed by Intent to Stay. Beyond these, segment-specific drivers emerge.
   - **Workforce Clustering - Thre Natural Segments**
     - The clustering analysis produced three actionable workforce segments. The segments materially differ on engagement level, performance, and tenure profile, which means each requires a different retention conversation.
    
2. **Recommended Action Plans**

| Priority | Theme | Interventions |
| --- | --- | --- |
| #1 | Well-being / Belonging | Audit workload distributions to surface chronic over-allocation, Train managers to spot early signs of burnout and disengagement, Establish regular 1:1 check-in as a standard team practice |
| #2 | Recognition / Belonging | Train managers to recognise meaningfully and equitably, Track milestones and contributions visibly at team level, Schedule regular check-ins focused on appreciation and feedback |
| #3 | Communication / Directon / Transparency / Prospects / Belonging/ | Increase transparency through leadership townhalls, Share a clear business stratefic roadmap regularly, cascade strategy narratives through people leaders so the mesafe reaches every team | 
| #4 | Growth / Prospects | Embed structured career conversations with individual development plans | Provide rotation, stretch assignments, and mentoring programmes, Publish transparent, criteria based promotion guidelines |

## Engagement Driver Dashboard
  **Dashboard**
  - File: [People Analytics Dasboard](https://github.com/brianohzg/HR_Employee-Enagagement-Attrition-Analytics-Project/blob/main/Dashboard_People%20Analytics.pbix)
  - The dashboad lists every engagement driver with its corresponding score, the correlation with overall engagement, and a calculated cpriority score that combines the gap-from-target with the correlation strenght such that drivers which are both low-scoring and highly correlated with engagement are ranked highest. This dashboard is catered specifically for HR business partner to support strategic conversations across different organization levels.
    <img width="1125" height="840" alt="image" src="https://github.com/user-attachments/assets/02f00513-45f3-480c-9375-a8f4cca57afb" />

## Limitations
  Several limitations and challenges should be knowledged when interpreting the findings.
  - Different survey structures between both years.
  - Low 2026 resonse rate.
  - Correlation does not imply causation.
  - Attrition events occurred before survey conducted.

---
                                                                                      Thank you for reading!
