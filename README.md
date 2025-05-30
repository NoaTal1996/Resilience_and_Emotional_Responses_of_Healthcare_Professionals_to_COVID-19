# Resilience_and_Emotional_Responses_of_Healthcare_Professionals_to_COVID-19
This repository contains data and code for replication of the results presented in the paper. 

Importantly, no individual-level data is provided as part of this repository. De-identified individual-level data can be attained for IRB-approved uses under the terms and conditions specified in the paper. 


* The folder `graphics` contains all figures shown in the paper.
* The `code` folder contains all Python scripts used to generate the figures 
  
## Fig 1: Emotion Trends

The `data/Fig_1` folder contains data used to generate Figure 1 in the main paper.

Both files include monthly emotion scores (means, standard deviations, confidence intervals) and a parsed `date` column, ranging from **2019-01-01** to **2022-05-01**.

- `hcp_graph1.csv`: Data for HCPs
- `nonhcp_graph1.csv`: Data for the non-HCPs


## Fig 2: Emotion Trends by Phase
The data/Fig_2 folder contains data used to generate Figure 2 in the main paper.

Both files include emotion scores aggregated by pandemic phase (mean, standard deviation, 95% confidence interval) and number of unique users per phase.

`hcp_stats_graph2.csv` : Data for HCPs

`nonhcp_stats_graph2.csv` : Data for the non-HCPs

### Fig 3: Correlation Between Emotions and Pandemic Progression

The `data/Fig_3` folder contains data used to generate Figure 3 in the main paper.

Each `.csv` file contains **weekly averages** of six basic emotions—**joy, sadness, anger, surprise, disgust, and fear**—for each population group:
- `weekly_stats_data_HCPs.csv`: Data for HCPs
- `weekly_stats_data_NonHCPs.csv`: Data for the non-HCP

The data is indexed by ISO week start date (`date`) and includes the following columns:
- `avg_joy`
- `avg_sadness`
- `avg_anger`
- `avg_surprise`
- `avg_disgust`
- `avg_fear`

These files were used to analyze the **correlation between population-level emotions and the progression of the COVID-19 pandemic** on a weekly basis.

## Fig 4: Hashtag Category Trends by Emotion

The `data/Fig_4` folder contains data used to generate Figure 4 in the main paper.

Each file is a single CSV file containing aggregated tweet counts from the top 10% most emotionally expressive tweets.  
The data is grouped by `emotion`, `date`, and `category`, with a corresponding count of tweets.

### File Format
Each row in the CSV contains:

- `emotion`: One of the four analyzed emotions – `joy`, `sadness`, `anger`, or `fear`  
- `date`: The date of the aggregated tweets (monthly)  
- `category`: The hashtag category assigned to the tweet  
- `count`: Number of tweets in that emotion-category-date combination  

### Files

- `category_hcp.csv`: Emotion-category trends for HCPs  
- `category_non_hcp.csv`: Emotion-category trends for the non-HCPs

### 📊 Cohen's d Effect Sizes by Phase and Emotion

The `data/Cohen_d` folder contains aggregated data used to compute **Cohen's d effect sizes** for emotional expressions (joy, sadness, anger, fear, surprise, disgust) across different COVID-19 phases. The effect sizes quantify the magnitude of emotional change relative to the baseline period ("Before COVID Phases").

Each file is a CSV file containing a table with the following columns:

- `phase`: One of the defined study periods (e.g., Phase 1, Phase 2, etc.)
- `unique_users`: Number of unique users per phase
- `<emotion>_mean`, `<emotion>_std`: Mean and standard deviation of each emotion
- `<emotion>_95ci`: 95% confidence interval for the emotion score (as a tuple)
- `<emotion>_cohen_d`: Cohen's d effect size, comparing each phase to the baseline
- `<emotion>_cohen_d_ci`: 95% confidence interval for the Cohen's d value (as a tuple)

### Files:
- `hcp_cohend.csv`: Statistics and effect sizes for the HCP 
- `nonhcp_cohend.csv`: Statistics and effect sizes for the non-HCP



### 🇺🇸 `owid-covid-data.csv` – U.S. COVID-19 Time Series Data

This CSV file contains daily COVID-19 data for the United States, extracted from the global dataset by Our World in Data.

**Key columns include:**
- `date`: Observation date  
- `new_cases`, `new_deaths`: Daily reported cases and deaths  
- `new_cases_smoothed`, `new_deaths_smoothed`: 7-day smoothed values  
- `total_cases`, `total_deaths`: Cumulative totals  
- `hosp_patients`, `icu_patients`: Current hospitalized and ICU patient counts  
- `weekly_hosp_admissions`, `weekly_icu_admissions`: New weekly hospital and ICU admissions  
- Demographics and healthcare capacity: `life_expectancy`, `hospital_beds_per_thousand`, `male_smokers`, etc.  
- Excess mortality estimates: `excess_mortality_cumulative`, `excess_mortality_per_million`, etc.
📥 [Download Data (Google Drive)](https://drive.google.com/file/d/15Gv8XX5FgwJpn15vikh9NyIa2W127yyY/view?usp=sharin)





## 🔗 Model Download

You can download the trained model from the following link:

📥 [Download Model (Google Drive)](https://drive.google.com/file/d/1OtI9ZQOkX3xgTiNTQdRoUHUsmPz7l3IP/view?usp=sharing)







