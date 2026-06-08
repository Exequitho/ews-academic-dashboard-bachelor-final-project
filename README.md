<div align="center">
  <h1>🚀 Academic Early Warning System (EWS) & Analytics Dashboard</h1>
  <p><i>Transforming fragmented academic data into proactive, rule-based interventions using Python & Looker Studio.</i></p>

  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/Looker_Studio-4285F4?style=for-the-badge&logo=looker&logoColor=white" alt="Looker Studio" />
  <img src="https://img.shields.io/badge/Data_Engineering-FF6F00?style=for-the-badge&logo=google-cloud&logoColor=white" alt="Data Engineering" />

  <br /><br />
  <img src="img/TA - Dashboard.png" alt="Dashboard View" width="600px" />
</div>

<br />

<table>
  <tr>
    <td>
      <div align="center">
        <h2>Executive Summary</h2>
      </div>
      <p><b>The Problem:</b> The Information Systems Study Program (PRODI SI) at <b>STT Terpadu Nurul Fikri</b> relied on a fragmented, manual tracking system (SISKA) that failed to proactively identify students at risk of delayed graduation or dropout.</p>
      <p><b>The Solution:</b> Collaborating directly with program leadership (<b>Mrs. Misna</b>, Head of PRODI SI) and end-users (<b>Mrs. Shelly</b>), I engineered a fully automated <b>Early Warning System (EWS)</b>. Executed via the <b>Business Intelligence (BI) Roadmap</b>, the pipeline extracts and evaluates student data against strict academic thresholds to trigger proactive counseling interventions.</p>
    </td>
  </tr>
</table>

<br />

### **🛠️ Technical Architecture & Core Competencies**
* **Data Engineering & ETL:** Python (`Pandas`) utilized for complex data wrangling, handling missing values, and executing multi-table `LEFT JOIN` operations across disparate datasets (KHS, IPK, and Personal Data).
* **Data Quality Assurance (QA):** Conducted rigorous edge-case testing and anomaly detection, successfully identifying critical null values previously hidden in the source system.
* **Logic-Based Evaluation:** Designed strict algorithmic thresholds (e.g., GPA < 2.75, accumulation of D/E grades) to categorize students into explicit risk tiers.
* **BI Visualization:** Engineered interactive UI/UX in Google Looker Studio, successfully passing <b>100% of Black Box Testing</b> across 16 dynamic filtering features.
* **Stakeholder Management:** Elicited requirements and translated qualitative academic needs into strict, actionable business logic.

---

<div align="center">
  <h2>Visualizations & Key Metrics</h2>
</div>

<table>
  <tr>
    <td valign="top" width="50%">
      <div align="center">
        <h3>1. Average Semester GPA (IPS) Trend</h3>
        <img src="img/TA - Line Chart.png" alt="Line Chart IPS" width="400px" />
      </div>
      <br />
      <ul>
        <li><b>Metric Monitored:</b> Semester-over-Semester IPS (Indeks Prestasi Semester).</li>
        <li><b>Analysis:</b> This line chart visualizes the average academic performance trajectory across semesters 1 through 5, allowing stakeholders to pinpoint exact periods where student performance drops systemically.</li>
      </ul>
    </td>
    <td valign="top" width="50%">
      <div align="center">
        <h3>2. Graduation Risk Distribution</h3>
        <img src="img/TA - Bar Chart Angkatan.png" alt="Bar Chart Risk" width="300px" />
      </div>
      <br />
      <ul>
        <li><b>Metric Monitored:</b> Distribution of students across risk categories.</li>
        <li><b>Analysis:</b> Driven by Python logic that flags students based on strict thresholds (e.g., GPA < 2.75 or accumulating "D" and "E" grades), this chart serves as the core Early Warning System.</li>
      </ul>
    </td>
  </tr>
</table>

<br />

### **🔍 Findings & Insights**

**1. Data Integration & System Reliability**
* Through robust data cleaning using Python, I successfully consolidated multiple datasets that were previously isolated. **Black Box Testing** confirmed a **100% success rate across 16 interactive features** (including complex slicers for Batch, Semester, and Academic Advisor), proving the system's technical stability.

**2. Stakeholder Usability & Data Quality Gaps**
* During Qualitative Usability Testing with **Mrs. Misna** and **Mrs. Shelly**, the dashboard effectively served its core purpose. However, the high-level visualization exposed underlying data entry issues from the source system—specifically, **2 students were identified with null (missing) Academic Advisor (PA) data** that had previously gone unnoticed in the manual SISKA system.
* Learnability was high; as noted by **Bu Shelly**, once the filter interactions were briefly explained, the users could navigate the dashboard and execute complex queries seamlessly.

---

### **📈 Actionable Recommendations**

Based on the quantitative metrics and qualitative insights gathered during the deployment phase, I presented the following recommendations to the stakeholders:

* **Address the Missing Data Anomaly:** Because the dashboard successfully flagged **2 instances of missing Academic Advisor data**, I recommend the administrative team audit the SISKA input protocol to ensure 100% data completeness at enrollment.
* **Implement Targeted Interventions:** Utilizing the exact data from the **Bar Chart Risk Distribution**, **Misna Asqia** and the academic advising team should immediately initiate one-on-one counseling for students identified in the high-risk category before the next semester begins.
* **Scale the Solution:** Given the **16 out of 16 feature success rate** and positive reception, I recommend scaling this dashboard to other study programs (such as TI and BD) to create a unified institutional monitoring standard.
