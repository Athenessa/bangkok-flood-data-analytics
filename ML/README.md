# Our goal is
"Given a fixed budget, 
how should Bangkok allocate its flood-management budget across districts to reduce flood risk?"

## Note
Seven district records have missing average flood duration because no flood events were recorded during the observation period. These values were retained as missing rather than imputed as zero, since average duration is undefined when there are no recorded events. All seven districts were retained for further analysis.

## WorkFlow
Stage A — Machine Learning
Combine district budget data and flood observations


Feature engineering

Create district-level flood characteristics


Feature scaling

StandardScaler


K-Means clustering

Group districts with similar flood characteristics


Evaluate and interpret clusters

Elbow method, silhouette score, cluster profiles


Stage B — Budget Optimization
Use district risk profiles and existing budget data
- use this https://analysisfunction.civilservice.gov.uk/policy-store/an-introductory-guide-to-mcda/



Define budget constraints and intervention scenarios


Optimization model

Allocate a fixed budget under explicit assumptions


Compare current and proposed allocations
