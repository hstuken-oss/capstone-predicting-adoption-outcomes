### Predicting Shelter Animal Adoption Outcomes ###

## Project Overview
*   This capstone project analyzes intake and outcome data from the Austin Animal Center to predict whether a dog or cat will be adopted, returned to its owner, transferred, or face euthanasia based on characteristics present at the time of intake.

## Buisness Problem
*   Animal shelters across the United States operate under persistent resource constraints — limited kennel space, staffing shortages, and finite funding — that make it difficult to give equal attention to every animal in their care. The Austin Animal Center, one of the largest municipal no-kill shelters in the United States, intakes thousands of dogs and cats annually and is committed to maintaining high live release rates. However, identifying which animals are most at risk of poor outcomes before those outcomes occur remains a significant operational challenge. Without a data-driven approach, shelter staff must rely on experience and intuition when deciding which animals to prioritize for interventions such as foster placement, increased marketing exposure, or behavioral support. Animals that would benefit most from targeted action are not always identified in time, leading some to remain in the shelter for extended periods or ultimately face poor outcomes that earlier intervention might have prevented.
*   This project addresses that gap by analyzing over 178,000 historical intake and outcome records from the Austin Animal Center to identify which animal characteristics — including age, breed, color, intake type, and length of stay — most strongly predict whether a dog or cat will be adopted, returned to its owner, transferred, or face euthanasia. The resulting random forest classification model achieved 76% accuracy and identified length of stay, age upon intake, and coat color as the three strongest predictors of adoption outcomes, providing shelter administrators with actionable, data-driven insights to prioritize limited resources toward at-risk animals and improve live release rates.

## Reasearch Question
*   Which animal characteristics — including species, age, breed, color, sex, neuter status, intake type, intake condition, and length of stay — most strongly predict whether a dog or cat admitted to the Austin Animal Center will be adopted, returned to owner, transferred, or face euthanasia?

## Key Findings
- Model achieved 76% overall accuracy across 4 outcome categories
- Length of Stay is the strongest predictor of adoption outcome (30% importance)
- Age upon Intake is the second strongest predictor (14% importance)
- Color is the third strongest predictor (13% importance) — supporting black cat syndrome research
- Breed ranked fourth (12% importance) — bully breeds show consistently higher transfer rates
- Dogs are significantly more likely to be returned to their owner than cats
- Cats leave the shelter faster than dogs across almost every outcome category

## Model Performance
| Outcome Category | Precision | Recall | F1-Score |
|---|---|---|---|
| Adopted | 0.77 | 0.92 | 0.83 |
| Returned to Owner | 0.82 | 0.73 | 0.77 |
| Transferred | 0.73 | 0.56 | 0.63 |
| Other | 0.56 | 0.28 | 0.37 |
| **Overall Accuracy** | | | **0.76** |

## Recommendations
1. **Implement a Length of Stay Early Intervention Program** — Automatically flag animals 
after seven days in the shelter for targeted action including foster placement referrals, 
social media promotion, and adoption event inclusion. The first week is the critical 
intervention window.

2. **Develop Targeted Adoption Initiatives for High-Risk Profiles** — Create age-specific 
promotions for senior animals, improve photography practices for dark-coated animals, and 
remove breed labels for mixed breed dogs in favor of behavioral descriptions to reduce 
adoption bias.

## Data Source
* This capstone project analyzes the intake and outcome data from the Austin Animal Center in Austin, Texas.
* Austin Animal Center — City of Austin Open Data Portal

- Intakes Dataset - https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Intakes/wter-evkm

- Outcomes Dataset - https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Outcomes/9t4d-g238

## Tools and Technologies
- Python 3.12.3
- pandas, scikit-learn, matplotlib, seaborn
- SQL/ SQLite
- Jupyter Notebook
- VS Code

## Methodology
This project followed the CRISP-DM (Cross Industry Standard Process for Data Mining) methodology across six phases: Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment.

## Dataset Summary
- 178,122 records after cleaning and preparation
- Spanning October 2013 through May 2025
- Dogs and cats only
- 9 predictor variables
- 4 outcome categories

## Project Structure
- 'capston.ipynb' -Main analysis notebook
- 'README.md' -Project overview and documentation
- 'Forms/' -WGU capstone approval and release forms
- 'Capstone Report/' -Written reports for Task 2 and Task 3
- 'charts' -.png images of all the visulations produced

## Author
Heather Stukenbroeker
Western Govenors University - B.S. Data Analytics Capstone



## Related Research
This project was informed by published research on shelter animal outcomes including:
- Powell et al. (2021) — Age and breed as predictors of shelter returns
- Jardim et al. (2026) — Length of stay as the strongest predictor of adoption
- Villarreal et al. (2026) — Coat color bias and black cat syndrome
- Svoboda & Hoffman (2015) — Breed and age effects on shelter dog outcomes
- Reese (2021) — Shelter programs and live release rates
- Parte (2019) — Machine learning on Austin Animal Center data