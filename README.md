# Resilience_and_Emotional_Responses_of_Healthcare_Professionals_to_COVID-19
This repository contains data and code for replication of the results presented in the paper. 

Importantly, no individual-level data is provided as part of this repository. De-identified individual-level data can be attained for IRB-approved uses under the terms and conditions specified in the paper. 


* The folder graphics contains all figures shown in the paper.
  
## Fig 1: Emotion Trends

The `data/Fig_1` folder contains data used to generate Figure 1 in the main paper.

Both files include monthly emotion scores (means, standard deviations, confidence intervals) and a parsed `date` column, ranging from **2019-01-01** to **2022-05-01**.

- `hcp_graph1.csv`: Data for HCPs
- `nonhcp_graph1.csv`: Data for the non-HCPs


## Fig 2: Emotion Trends by Phase
The data/Fig_2 folder contains data used to generate Figure 2 in the main paper.

Both files include emotion scores aggregated by pandemic phase (mean, standard deviation, 95% confidence interval) and number of unique users per phase.

hcp_stats_graph2.csv : Data for HCPs

nonhcp_stats_graph2.csv : Data for the non-HCPs


## Fig 4: Hashtag Category Trends by Emotion

The `data/Fig_4` folder contains data used to generate Figure 4 in the main paper.

Each file is a pickled Python dictionary, where:
- The **keys** are emotions: `joy`, `sadness`, `anger`, `fear`  
- The **values** are DataFrames containing tweet counts grouped by `date` and `category`

These counts represent the number of tweets in each category extracted from the top 10% most emotionally expressive tweets for that emotion.

### Files:
- `category_non_hcp.pkl`: Dictionary for the non-HCPs 
- `category_hcp.pkl`: Dictionary for HCPs

### 📊 Cohen's d Effect Sizes by Phase and Emotion

This folder contains aggregated data used to compute **Cohen's d effect sizes** for emotional expressions (joy, sadness, anger, fear, surprise, disgust) across different COVID-19 phases. The effect sizes quantify the magnitude of emotional change relative to the baseline period ("Before COVID Phases").

Each `.pkl` file contains a `pandas.DataFrame` with the following columns:

- `phase`: One of the defined study periods (e.g., Phase 1, Phase 2, etc.).
- `unique_users`: Number of unique users per phase.
- `<emotion>_mean`, `<emotion>_std`: Mean and standard deviation of each emotion.
- `<emotion>_95ci`: 95% confidence interval for the emotion score (tuple).
- `<emotion>_cohen_d`: Cohen's d effect size, comparing each phase to the baseline.
- `<emotion>_cohen_d_ci`: 95% confidence interval for the Cohen's d value (tuple).

**Files:**
- `hcp_stats_cohend.pkl`: Statistics and effect sizes for the HCP population.
- `nonhcp_cohend.pkl`: Statistics and effect sizes for the non-HCP population.







## 🔗 Model Download

You can download the trained model from the following link:

📥 [Download Model (Google Drive)](https://drive.google.com/file/d/1OtI9ZQOkX3xgTiNTQdRoUHUsmPz7l3IP/view?usp=sharing)




