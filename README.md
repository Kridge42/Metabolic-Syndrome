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

The default random forest model was my best performing model with the given dataset.

![Screenshot (49)](https://user-images.githubusercontent.com/126993169/236969489-96ec3b2c-44f1-4882-81a4-c6dac9a01470.png)

The training set runs perfect predictions but the test set produces overall accuracy of 88%. The test set does very well predicting those who do not have metabolic syndrome. However, the predicition of those who do have metabolic syndrome is at 77%. This means that 23% were predicted to have metabolic syndrome but actually did not. Also, 7% were predicted to be negative but were actually positive for metabolic syndrome. 

# Recommendations

I believe the model findings could modestly predict metabolic syndrome but only because the dataset used is subpar. The first issue is the very small sample of data that is also unbalanced. The next issue is that a major feature, blood pressure measurements, isn't even included in this data. More data would definitely lead to a better predictive quality model.

The visuals do provide an accurate representation for the factors contributing to metabolic syndrome as per listed levels at the cdc, heart.org, and the mayo clinic. That being said, there were many features listed here that provided very little, if any, relevance to who will develop metabolic syndrome.

Thoughts to include for a larger data sample:
- Include activities or habits that are proven to increase or decrease HDL levels.
- List behaviors of participants such as binge eating, screen time, exercise levels, smoking  and alcohol intake, etc.
- In place of monthly income and marital status; I would like to see calories consumed daily, height, weight, and body fat percentage. 
- Ask each participant their stress level 1 to 10. 

 

 

 

 

 
NOTES: ATP III is Adult Treatment Panel III. Table taken from: Grundy SM, Brewer HB, Cleeman JI, Smith SC, Lenfant C.
Definition of metabolic syndrome. Report of the National Heart, Lung, and Blood Institute/American Heart Association Conference
on scientific issues related to definition. Circulation. 109:433–8. 2004(2

Data Dictionary
