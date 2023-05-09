# Predicting Metabolic Syndrome

- Author: Kevin Ridge

## Goal for Project:
- Create machine learning models to predict if someone has metabolic syndrome.

This data comes from the National Center for Statistics.

link to data.world source: https://data.world/informatics-edu/metabolic-syndrome-prediction

## Data Dictionary

![image](https://user-images.githubusercontent.com/126993169/236963130-12b3ab17-c298-437b-8317-c02df82299bd.png)

## What is metabolic syndrome? 
### Metabolic syndrome is a group of five conditions that can lead to heart disease, diabetes, stroke and other health problems. 
### Metabolic syndrome is diagnosed when someone has three or more of these risk factors: 

- High blood glucose (sugar). 
  - Fasting glucose: ≥100 mg/dL
- High levels of triglycerides in the blood.
  -  Triglycerides: ≥150 mg/dL.
- High blood pressure 
  - Blood pressure: ≥135/≥85 mm Hg
- Large waist circumference or “apple-shaped” body.
  - Men  >102 cm (>40 in)
  - Women  >88 cm (>35 in)
- Low levels of HDL (“good”). cholesterol in the blood. 
  -  Men <40 mg/dL
  -  Women <50 mg/dL

- Source: https://www.heart.org/en/health-topics/metabolic-syndrome/about-metabolic-syndrome
- Source: https://www.cdc.gov/nchs/data/nhsr/nhsr013.pdf

# Data Analysis

This data set contains no blood pressure measurements. One of the five conditions measured to diagnose metabolic syndrome will not even be considered in this dataset. Along with the missing blood pressure readings, the dataset is very small, only 2401 participants. From the 2401 participants, only 34% or 816 were determined positive, this means the data is very imbalanced. 

These are major challenges for the predictive quality for the machine learning models. 

# ## **Evaluation of visuals**

![image](https://user-images.githubusercontent.com/126993169/236965207-f0f9fd4e-4706-499e-8e1c-26c46e9bb1e6.png)
- The positive (1) cases of metabolic syndrome almost exclusively exceed the 100 mg/dl for fasting blood glucose. Also worth noting, is that a high percentage of positive instances are above the 150 mg/dL for triglycerides.

![image](https://user-images.githubusercontent.com/126993169/236965018-815d9807-2351-40b9-b975-15da9e3d19df.png)
- The bulk of positive (1) cases of metabolic syndrome are shown here with a BMI above 28 and a waist circumference above 90 centimeters. 

![image](https://user-images.githubusercontent.com/126993169/236965050-f206e0a5-3676-4531-b16f-f38f72b50210.png)
- The positive (1) cases of metabolic syndrome are shown to have what is considered to be an overweight or obese BMI. In contrast, the negative (0) cases for metabolic syndrome are closer to what is considered to be in the normal BMI range.

![image](https://user-images.githubusercontent.com/126993169/236965084-5a73078f-8a17-455c-be7f-f1197997d344.png)
- Most of the positive (1) cases of metabolic syndrome measured at less than 60 for the beneficial cholesterol known as HDL mg/dL. 

### Random forest model

![image](https://user-images.githubusercontent.com/126993169/236968481-4539b50e-e688-49c2-b8d1-bcea86505ac8.png)

![image](https://user-images.githubusercontent.com/126993169/236968913-b3d52efe-8051-4b54-bded-34aaee683406.png)





Create a README.md file in your GitHub repository.  This README should include:
Your business problem and stakeholders
The source of your data
A description of your data
2 analytical insights from your data analysis.  
You can use the 2 plots from Project 2, part 3 for this!
They should include visualizations AND written interpretations
The metrics for your best model
A description of how well your model would solve your business problem
A summary with at least 2 recommendations for your stakeholders, based on your model performance AND analytical findings.

 

 

 

 

 
NOTES: ATP III is Adult Treatment Panel III. Table taken from: Grundy SM, Brewer HB, Cleeman JI, Smith SC, Lenfant C.
Definition of metabolic syndrome. Report of the National Heart, Lung, and Blood Institute/American Heart Association Conference
on scientific issues related to definition. Circulation. 109:433–8. 2004(2

Data Dictionary
