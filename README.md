### Predicting Shelter Animal Adoption Outcomes ###

## Project Overview
*   This capstone project analyzes the intake and outcome data from the Austin Animal Center in Austin, Texas. The data is used to predict whether a dog or cat will be adopted, returned to its owner, or euthanized, based on charcteristics present at the time of intake.

## Buisness Problem
*   Animal shelters operate with limited staff, space, and resources. This project builds a classification model to help shelter administrators identify at-risk animals earlier and maintaining their goal of sustaining high live release rates.

## Reasearch Question
*   Which animal characteristics (including species, age, breed, color, sex, neuter status, and intake condition) most strongly predict the adoption outcome for dogs and cats at the Austin Animal Center?

## Data Source
* Austin Animal Center — City of Austin Open Data Portal

- Intakes Dataset - https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Intakes/wter-evkm

- Outcomes Dataset - https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Outcomes/9t4d-g238

## Tools and Technologies
- Python 3.12.3
- Pandas, scikit-learn, matplotlib, seaborn
- SQL/ SQLite
- Jupyter Notebook
- VS Code

## Key Findings
*   The Random Forest Model achieved 76% accuracy across 4 outcome categories
*   Length of Stay is the *Strongest* predictor of adoption outcome (30% Importance)
*   Age upon Intake is the second strongest predictor (14% importance)
*   Color and Breed are significant predictors supporting the black cat syndrome theory
*   Dogs are significantly more likely to be returned to their owners than cats

## Project Structure
- 'capston.ipynb' -Main analysis notebook
- 'README.md' -Project overview and documentation
- 'Forms/' -WGU capstone approval and release forms
- 'Capstone Report/' -Written reports for Task 2 and Task 3

## Author
Heather Stukenbroeker
Western Govenors University - B.S. Data Analytics Capstone