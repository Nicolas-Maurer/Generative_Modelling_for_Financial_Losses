# Generative_Modelling_for_Financial_Losses
This directory contains my approach, my reasoning and my results for the tournament "Generative_Modelling_for_Financial_Losses" sponsored by "Ecole Polytechnique" and "BNP Paribas"  

Link of the competition : https://competitions.outcoder.ai/competitions/genm

# Context
In the last two decades, the increasing number of shocks and financial crises has been a major issue for the financial risk management teams.

Among the wide range of exercises in this field, Stress tests have become a main guideline for the regulator in order to assess the banking system resilience against the realizations of various categories of risk (market, credit, operational, climate, etc). The main challenge is to simulate unfavorable extreme (but plausible) negative returns similar to a historical dataset.

# The Task
This is an unsupervised learning problem: Given real data from stock market indexes that will act as a train dataset, the task is to learn a generative model that simulates synthetic stock market indexes.

The difficulty mainly lies in two points :  
a) find an appropriate transformation to generate extreme values for some given input noise.  
b) learning a generative model based on a dataset which contains very few extreme data.

# Evaluation metrics 
The two evaluation metrics are: 
- How well you will fit the marginals (Anderson-Darling)
- How well you will fit the dependence structure between market indexes (Absolute Kendall Error)
