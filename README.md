# Resilience_and_Emotional_Responses_of_Healthcare_Professionals_to_COVID-19
This repository contains data and code for replication of the results presented in the paper. 

Importantly, no individual-level data is provided as part of this repository. De-identified individual-level data can be attained for IRB-approved uses under the terms and conditions specified in the paper. 


* The folder graphics contains all figures shown in the paper.
  
## Fig 1: Emotion Trends

The `data/Fig_1` folder contains data used to generate Figure 1 in the main paper.

Both files include monthly emotion scores (means, standard deviations, confidence intervals) and a parsed `date` column, ranging from **2019-01-01** to **2022-05-01**.

- `hcp_graph1.csv`: Data for health care professionals (HCPs)
- `nonhcp_graph1.csv`: Data for the general population (non-HCPs)


## Fig 2: Emotion Trends by Phase
The data/Fig_2 folder contains data used to generate Figure 2 in the main paper.

Both files include emotion scores aggregated by pandemic phase (mean, standard deviation, 95% confidence interval) and number of unique users per phase.

hcp_stats_graph2.csv : Data for health care professionals (HCPs)

nonhcp_stats_graph2.csv : Data for the general population (non-HCPs)


## Fig 4: Hashtag Category Trends by Emotion

The `data/Fig_4` folder contains data used to generate Figure 4 in the main paper.

Each file includes quarterly frequencies of hashtag categories extracted from the top 10% most emotionally expressive tweets.  
Tweets are grouped by `date` and `category`, with counts representing the number of tweets per category.

- `hcp_hashtag_counts.csv`: Data for health care professionals (HCPs)  
- `nonhcp_hashtag_counts.csv`: Data for the general population (non-HCPs)




## 🔗 Model Download

You can download the trained model from the following link:

📥 [Download Model (Google Drive)](https://drive.google.com/file/d/1OtI9ZQOkX3xgTiNTQdRoUHUsmPz7l3IP/view?usp=sharing)




