<div align="center">
  <h1 align="center">Academic Dashboard for On-Time Graduation Monitoring</h1>
  
  <img src="img/TA - Dashboard.png" alt="Dashboard View" width="600px" />
</div>

<br />

<table>
  <tr>
    <td>
      <div align="center">
        <h2>Client Background & Problem Statement</h2>
      </div>
      <p><b>PRODI SI (Information Systems Study Program)</b> at <b>STT Terpadu Nurul Fikri</b> faced significant challenges in monitoring student academic progress. The existing process relied heavily on manual tracking via the SISKA system, which caused inefficiencies, fragmented data, and an inability to proactively identify students at risk of delayed graduation.</p>
      <p>Working closely with key stakeholders, including <b>Misna Asqia</b> (Head of PRODI SI) and <b>Bu Shelly</b> (End-User Evaluator), I developed an automated <b>Early Warning System (EWS)</b> and Academic Dashboard utilizing the <b>Business Intelligence (BI) Roadmap</b> methodology to streamline operations and prevent student dropouts.</p>
    </td>
  </tr>
</table>

<br />

### **Core Competencies Demonstrated**
* **Data Engineering & ETL:** Utilized Python (Pandas) for cleaning and executing `left join` operations on complex, fragmented datasets (Personal Data, Study Results/KHS, and GPA/IPK).
* **Data Visualization:** Engineered interactive UI/UX in Google Looker Studio.
* **Framework & Project Management:** Executed end-to-end lifecycle using the Business Intelligence (BI) Roadmap (Justification, Planning, Analysis, Design, Construction, Deployment).
* **Quality Assurance:** Conducted exhaustive Black Box Testing and Qualitative Usability Testing.
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

### **Findings & Insights**

**1. Data Integration & System Reliability**
* Through robust data cleaning using Python, I successfully consolidated multiple datasets that were previously isolated. **Black Box Testing** confirmed a **100% success rate across 16 interactive features** (including complex slicers for Batch, Semester, and Academic Advisor), proving the system's technical stability.

**2. Stakeholder Usability & Data Quality Gaps**
* During Qualitative Usability Testing with **Misna Asqia** and **Bu Shelly**, the dashboard effectively served its core purpose. However, the high-level visualization exposed underlying data entry issues from the source system—specifically, **2 students were identified with null (missing) Academic Advisor (PA) data** that had previously gone unnoticed in the manual SISKA system.
* Learnability was high; as noted by **Bu Shelly**, once the filter interactions were briefly explained, the users could navigate the dashboard and execute complex queries seamlessly.

---

### **Actionable Recommendations**

Based on the quantitative metrics and qualitative insights gathered during the deployment phase, I presented the following recommendations to the stakeholders:

* **Address the Missing Data Anomaly:** Because the dashboard successfully flagged **2 instances of missing Academic Advisor data**, I recommend the administrative team audit the SISKA input protocol to ensure 100% data completeness at enrollment.
* **Implement Targeted Interventions:** Utilizing the exact data from the **Bar Chart Risk Distribution**, **Misna Asqia** and the academic advising team should immediately initiate one-on-one counseling for students identified in the high-risk category before the next semester begins.
* **Scale the Solution:** Given the **16 out of 16 feature success rate** and positive reception, I recommend scaling this dashboard to other study programs (such as TI and BD) to create a unified institutional monitoring standard.
