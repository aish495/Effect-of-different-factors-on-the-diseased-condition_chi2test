#### **Effect of different factors on Disease Occurrence – Chi-Square Test Project**



Project Overview



This project explores whether lifestyle habits and demographic attributes (such as smoking, gender, and treatment assignment) are statistically associated with the occurrence of a disease. Using the Chi-Square Test of Independence, we test relationships between categorical variables in the dataset.



The project is implemented in Python (Jupyter Notebook) using pandas, scipy, and numpy.



**Dataset Description**



The dataset contains 40 records with the following attributes:



id – Unique identifier



gender – Male (M) or Female (F)



smoker – Yes / No



treatment – Assigned group (A or B)



disease – Yes / No (disease occurrence)



age – Age in years



bmi – Body Mass Index



systolic\_bp – Systolic blood pressure



cholesterol – Cholesterol level



glucose – Glucose level



activity\_mins – Daily activity in minutes



For the chi-square analysis, only categorical variables (gender, smoker, treatment, disease) are used.



**Methodology**



Contingency tables were created to summarize observed frequencies.



Expected frequencies were calculated under the assumption of independence.



The Chi-Square statistic (χ²), degrees of freedom, and p-value were computed using:



Chi-Square (χ²) = Σ ( (O - E)² / E )

Where:

O = Observed frequency

E = Expected frequency	​



Results were interpreted at a 5% significance level (α = 0.05).



**Key Results \& Interpretations**



1\. Smoking vs Disease



Contingency Table



disease   No   Yes

smoker

No        25    8

Yes        4     3



p-value = 0.592 (> 0.05)



Interpretation: Smoking status is not significantly associated with disease occurrence in this dataset.



2\. Treatment vs Disease



Contingency Table



disease     No   Yes

treatment

A            16    7

B            13    4



p-value = 0.900 (> 0.05)



Interpretation: The type of treatment (A or B) shows no significant effect on disease occurrence.



3\. Gender vs Disease



Contingency Table



disease   No   Yes

gender

F         14   11

M        15   0



p-value = 0.008 (< 0.05)



Interpretation: There is a statistically significant association between gender and disease occurrence.

Females are more likely to have the disease than expected.

Males are less likely to have the disease.

