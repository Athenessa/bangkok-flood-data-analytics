# Our goal is
"Given a fixed budget, 
how should Bangkok allocate its flood-management budget across districts to reduce flood risk?"

## Note
Seven district records have missing average flood duration because no flood events were recorded during the observation period. These values were retained as missing rather than imputed as zero, since average duration is undefined when there are no recorded events. All seven districts were retained for further analysis.

## WorkFlow
START: Bangkok Flood Dataset
budget + flood + historical impact


1. Data Preparation
Clean, encode, handle missing values, check duplicates


2. Feature Engineering
Aggregate flood observations into 50 district-level records


3. Feature Selection and Scaling
Select flood-related variables and standardize their scales


4. K-Means Clustering
Group districts by similar flood characteristics


5. Model Evaluation
Choose number of clusters, inspect silhouette score and cluster profiles


6. District Risk Profiling
Interpret flood characteristics and identify district priorities


7. Budget Optimization
Allocate a fixed budget subject to constraints and estimated intervention effectiveness


FINAL: Compare Budget Allocation Strategies
Current allocation vs proposed allocation
