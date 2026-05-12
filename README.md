# Ivy_Liu_Final_Project
This project uses a public ecological momentary assessment (EMA) dataset to examine repetitive negative thinking (RNT) in daily life. The dataset was obtained from the Open Science Framework (OSF) and includes baseline questionnaire measures, EMA assessments, multiple follow-up assessments, and different experimental conditions.

For the current project, only participants in the no mental health assistance condition were included. The analyses focused on baseline questionnaire measures and EMA data. The main purpose of this project is to examine whether EMA-based measurements and baseline trait measures reflect similar patterns of repetitive negative thinking, and to investigate which EMA indices are more strongly associated with depression and anxiety symptoms.

## Instructions to Run the Code
1. Download the dataset file (`Data_filtered_osf_final.csv`) from the OSF project page (https://osf.io/dm2ab/files/osfstorage) and place it in the same folder as the R script.
2. Open the R script in RStudio.
3. Install the required packages if they are not already installed.
4. Run the script from top to bottom to reproduce the data cleaning, correlation analyses, and regression analyses.

## Research Questions
Are baseline trait repetitive negative thinking measures (rumination and worry) associated with EMA-based repetitive negative thinking indices in daily life? Which EMA-based repetitive negative thinking indices are more strongly associated with depression and anxiety symptoms?

## Variables
Baseline Variables
- rrs_total_0: baseline trait rumination score
- pswq_total_0: baseline trait worry score
- phq_total_0: baseline depressive symptom score
- gad_total_0: baseline anxiety symptom score
EMA Variables
- EMA_RNT_av: average repetitive negative thinking across EMA time points
- RNT_SD: variability (standard deviation) of repetitive negative thinking across EMA time points

## Main Analyses
- Data cleaning 
- EMA data aggregation
- Correlation analyses
- Multiple linear regression analyses

## Software and Packages
- R
- dplyr

## Findings
### Correlation Analyses
<img width="1206" height="272" alt="image" src="https://github.com/user-attachments/assets/ef54e5e9-c3a6-43c8-a9e9-7e87be51c368" />
Trait rumination was positively correlated with average EMA repetitive negative thinking (r = .36) and EMA variability (r = .32). Similarly, trait worry was positively correlated with average EMA repetitive negative thinking (r = .42) and EMA variability (r = .35).

In addition, average EMA repetitive negative thinking showed stronger positive associations with depressive symptoms (r = .38) and anxiety symptoms (r = .44) than EMA variability (depression: r = .20; anxiety: r = .32).

### Linear Regression
<img width="1082" height="697" alt="image" src="https://github.com/user-attachments/assets/234a529b-e3ea-4e79-bda1-8dd464c7632c" />

Both trait rumination and trait worry were significantly positively associated with average EMA repetitive negative thinking. Higher rumination scores (b = 0.30, p < .001) and higher worry scores (b = 0.20, p < .001) were associated with greater average repetitive negative thinking in daily life. Together, the two trait measures explained approximately 20% of the variance in average EMA repetitive negative thinking (R² = .20).

<img width="996" height="709" alt="image" src="https://github.com/user-attachments/assets/817c6ee6-eef7-424a-85dc-1974bfc14443" />

Both trait rumination and trait worry were significantly positively associated with variability in EMA repetitive negative thinking. Higher rumination scores (b = 0.13, p = .005) and higher worry scores (b = 0.07, p < .001) were associated with greater fluctuations in repetitive negative thinking across daily-life EMA assessments. Together, the two trait measures explained approximately 14% of the variance in EMA repetitive negative thinking variability (R² = .14).

<img width="820" height="598" alt="image" src="https://github.com/user-attachments/assets/2c1749ec-bc54-4593-aa31-33ed2db23998" />

Average EMA repetitive negative thinking was significantly positively associated with depressive symptoms. Higher average levels of repetitive negative thinking in daily life were associated with greater depressive symptoms (b = .30, p < .001). In contrast, EMA variability was not significantly associated with depressive symptoms after accounting for average EMA repetitive negative thinking (b = .02, p = .806). Together, the EMA indices explained approximately 14% of the variance in depressive symptoms (R² = .14).


<img width="824" height="597" alt="image" src="https://github.com/user-attachments/assets/e05f7a1a-08f4-414b-a706-e1d281f6e635" />

Both average EMA repetitive negative thinking and EMA variability were significantly positively associated with anxiety symptoms. Higher average levels of repetitive negative thinking in daily life (b = 0.30, p < .001) and greater variability in repetitive negative thinking (b = 0.22, p = .017) were associated with higher anxiety symptoms. Together, the EMA indices explained approximately 20% of the variance in anxiety symptoms (R² = .20).
