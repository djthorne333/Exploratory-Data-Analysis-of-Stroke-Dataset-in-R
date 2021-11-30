# Exploratory Data Analysis of Stroke Dataset in R 

### Author: datadave333@gmail.com

## Description of Data

*The dataset is from Kaggle, called "Stroke Prediction Dataset", found at this link: https://www.kaggle.com/fedesoriano/stroke-prediction-dataset.*   

*How this dataset was obtained, and the details of how each feature was measured is deemed "confidential" by the author. There are features 11 features related to life and health status: gender, age, hypertension, heart_disease, ever_married,	work_type, Residence_type,	avg_glucose_level, bmi, smoking_status, stroke.*  

*Catagorical: gender, ever_married, work_type, Residence_type, smoking_status  
One-hot:  hypertension, heart_disease, stroke, (Yes=1, No=0)  
Numerical: avg_glucose_level, bmi, age.*




## To Run:
*Under "Importing and data summary", enter the file path to the csv titled "healthcare-dataset-stroke-data" (included in repo, or grab from Kaggle using the link above).*

## EDA Results

### Strongest Correlation between numerical features was between age and bmi at 0.33, which is relatively weak:

![corrplot](https://user-images.githubusercontent.com/73368743/144136036-3cf27517-cd81-427b-9b5f-240347d84c91.png)

### All but gender and residence type were shown to be significant with regards to stroke (p-values well below 0.05 after chi2 test). The following features showed the highest range of stroke percentages across their values (1 = had stroke): 

![agebars](https://user-images.githubusercontent.com/73368743/144135955-549fc0e0-b430-44a8-8f13-9417537fd2cb.png)

![htbars](https://user-images.githubusercontent.com/73368743/144135983-7695f44d-e902-4a64-8792-966d8bf1c050.png)

![glucbars](https://user-images.githubusercontent.com/73368743/144136012-b2c880f3-fa85-47b3-8a70-fdfac1c14a5b.png)

![hdbars](https://user-images.githubusercontent.com/73368743/144136018-defe1020-f135-43dd-a3e1-a2d26a72b73d.png)

### From Multi-Level Density Plots:

* Most of the high glucose sample is populated by either children or people over 50 years old.
* Most of our healthy bmi sample between 25 and 75 years old is populated by females. 
* There is a slight peak in the amount of people populating our overweight/obese samples at around 55 years old. 
* Besides adolescents, most of our formerly smoked sample is populated by people 50-80 years old. 
* Much of our currently smoking sample is populated by people working government jobs/self employed and 50-65 years old. 
* There are many underweight people working government jobs at 60 years old.
