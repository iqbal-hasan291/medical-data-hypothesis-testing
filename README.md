# Medical Data Hypothesis Testing
**Project Overview**
This project applies statistical hypothesis testing to a real-world medical dataset of breast cancer patients. The dataset includes patient Age,Histology, biomarker levels, tumour stages, receptor statuses and surgical treatments and Patient Status.The main objective is to test whether key clinical factors (such as tumour stage) are statistically associated with treatment decisions and patient outcomes.
**Methodology**
*1.	Data Cleaning (Python)*
⦁	Loaded the raw dataset in Python (pandas).
⦁	Normalised column names (removed spaces, replaced with underscores).
⦁	Checked and handled missing values.
⦁	Converted categorical variables to consistent formats.
*2.	Hypothesis Testing (Google Colab)*
⦁	Used cross-tabulation and Chi-square tests to evaluate associations between:
⦁	Tumour Stage ↔ Surgery Type
⦁	HER2 receptor status ↔ Patient Status
⦁	Checked normality of numeric variables.
⦁	Applied the correct test depending on variable types (categorical vs. numerical).
3.	Visualisation & Reporting
⦁	Created grouped bar charts for surgery type by tumour stage.
⦁	Created grouped pie charts for HER2 receptor status by PatientStatus.
⦁	Summarised p-values and statistical decisions in a results table.
**Key Findings**
⦁	Tumour stage and surgery type:
Chi-square test showed a statistically significant association (p < 0.05). Later stages were more likely to undergo more radical surgery types.
⦁	HER2 receptor status and patient status:
Chi-square test also showed a significant association (p < 0.05). Higher tumour stages corresponded to worse patient outcomes at last follow-up.
**Recommendations**
⦁	Clinical planning: Findings support stage-based surgical decision-making and can inform resource allocation for more complex surgeries at later stages.
⦁	Data collection: Future datasets should include treatment follow-up times and additional biomarkers to strengthen survival analysis.
⦁	Statistical approach: Non-normal biomarker distributions suggest using non-parametric or transformed data for more accurate inference.

