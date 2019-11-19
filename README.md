# Data-visualization-and-preprocessing-of-AMEO-2015-Dataset
Data visualization and pre-processing of Aspiring Minds' Employability Outcomes 2015 (AMEO 2015) Dataset using Python.

## About the dataset

Aspiring Minds' Employability Outcomes 2015 (AMEO 2015), a unique dataset which provides engineering graduates' employment outcomes (salaries, job titles and job locations) together with standardized assessment scores in three fundamental areas - cognitive skills, technical skills and personality. Coupled with biodata information, AMEO 2015 provides an opportunity for a unique and comprehensive study of the entry level labor market.

The dataset used for this project was taken from the "IKDD CoDS 2016 Data Challenge" which can be found here: http://research.aspiringminds.com/resources/ameo


## Data Preprocessing

Here are a few important pre-processing operations done in this project:

1.Removing outliers: rows with salary > 10,00,000 is less than 1% of the data. So these rows were removed.
 
2.Only year from the DOB column is retained. 

3.New columns GradAge and 12GradAge were introduced indicating the age  of person during graduation and 12th graduation. 
 
4.Missing values indicated by -1 was replaced with 0.
 
5.12board: The most frequent boards are “cbse”, “state”, “icse” and “n/a”. We reduced each to one of (cbse, state, n/a, icse) and then one-hot-encoded them.

6.The specialization column data was mapped to ‘CS’,’EC’,’ME’,’EL’,’CE’ and other.
 
7.CollegeGPA was converted from 10 point scale to 100 point scale.
 
8.Unnecessary columns such as JobCity,DOL,DOJ etc were dropped.
 
9.Categorical data such as gender,specialization,degree,12board was one hot encoded


 
