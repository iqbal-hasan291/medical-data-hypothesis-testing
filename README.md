#  Medical Data Hypothesis Testing  

A statistical analysis project applying hypothesis testing to a real-world breast cancer dataset.  
This repository demonstrates how hypothesis testing can be used to uncover relationships between key clinical factors, treatment decisions, and patient outcomes.

---

##  Project Overview  
This project applies **statistical hypothesis testing** to a medical dataset of breast cancer patients.  
The dataset includes:  

- Patient Age  
- Histology  
- Biomarker levels  
- Tumour stages  
- Receptor statuses (HER2, etc.)  
- Surgical treatments  
- Patient Status  

**Goal:**  
Test whether key clinical factors (e.g., tumour stage, receptor status) are statistically associated with treatment decisions and patient outcomes.

---

##  Methodology  

### 1️ Data Cleaning (Python)
- Loaded raw dataset into Python using **pandas**  
- Normalized column names (removed spaces, replaced with underscores)  
- Checked and handled missing values  
- Converted categorical variables into consistent formats

  ![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/8e1c864b3941982dfec82a5af30bb73e5ee932ba/image/Test1.png)

  ![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/8e1c864b3941982dfec82a5af30bb73e5ee932ba/image/test2.png)

### 3️ Visualization & Reporting  
- Created grouped **bar charts** for Surgery Type by Tumour Stage
![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/8e1c864b3941982dfec82a5af30bb73e5ee932ba/image/test1image.png)

- Created grouped **pie charts** for HER2 Receptor Status by Patient Status
![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/8e1c864b3941982dfec82a5af30bb73e5ee932ba/image/test2image.png)

- Summarized **p-values** and statistical decisions in a results table  

### 2️ Hypothesis Testing (Google Colab)
- Performed cross-tabulation and Chi-square tests to evaluate associations:  
  - **Tumour Stage ↔ Surgery Type**
  ![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/c60727cd93726860ac3c2c9b56169d1c39e66a51/image/test1statement.png)
  ![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/c60727cd93726860ac3c2c9b56169d1c39e66a51/image/test1result.png)

  - **HER2 Receptor Status ↔ Patient Status**
  ![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/c60727cd93726860ac3c2c9b56169d1c39e66a51/image/test2statement.png)
![](https://github.com/iqbal-hasan291/medical-data-hypothesis-testing/blob/c60727cd93726860ac3c2c9b56169d1c39e66a51/image/test2result.png)
- Checked normality of numeric variables  

---

##  Key Findings  

- **Tumour Stage and Surgery Type**  
  - *Since the p-value < 0.05, we reject the null hypothesis (H₀). This indicates that surgical decisions are dependent on tumour stage.*
  - Later stages were more likely to undergo more radical surgery types.  

- **HER2 Receptor Status and Patient Status**  
  - *Since the p-value > 0.05, we fail to reject the null hypothesis (H₀). This indicates that patient outcome is independent of HER2 receptor status in this dataset—there’s no                statistically significant relationship.* 
  - Whether a patient’s tumour was HER2-positive or not didn’t show a clear link to how the patient did afterwards — outcomes were about the same either way in this dataset.

---

##  Recommendations  

- **Clinical Planning:**  
  Stage-based surgical decision-making should inform resource allocation for more complex surgeries at later stages.  

- **Data Collection:**  
  Future datasets should include treatment follow-up times and additional biomarkers to strengthen survival analysis.  

- **Statistical Approach:**  
  This analysis shows how simple statistical tests can reveal where medical decisions already align with clinical factors (like stage) and where relationships are unclear (like HER2        status).

---  

