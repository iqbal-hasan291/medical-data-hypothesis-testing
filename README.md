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

### 2️ Hypothesis Testing (Google Colab)
- Performed cross-tabulation and Chi-square tests to evaluate associations:  
  - **Tumour Stage ↔ Surgery Type**  
  - **HER2 Receptor Status ↔ Patient Status**  
- Checked normality of numeric variables  
- Applied appropriate statistical tests based on variable types (categorical vs. numerical)  

### 3️ Visualization & Reporting  
- Created grouped **bar charts** for Surgery Type by Tumour Stage  
- Created grouped **pie charts** for HER2 Receptor Status by Patient Status  
- Summarized **p-values** and statistical decisions in a results table  

---

##  Key Findings  

- **Tumour Stage and Surgery Type**  
  - Chi-square test showed a statistically significant association (p < 0.05).  
  - Later stages were more likely to undergo more radical surgery types.  

- **HER2 Receptor Status and Patient Status**  
  - Chi-square test also showed a significant association (p < 0.05).  
  - Higher tumour stages corresponded to worse patient outcomes at last follow-up.  

---

##  Recommendations  

- **Clinical Planning:**  
  Stage-based surgical decision-making should inform resource allocation for more complex surgeries at later stages.  

- **Data Collection:**  
  Future datasets should include treatment follow-up times and additional biomarkers to strengthen survival analysis.  

- **Statistical Approach:**  
  Non-normal biomarker distributions suggest using non-parametric or transformed data for more accurate inference.  

---  

