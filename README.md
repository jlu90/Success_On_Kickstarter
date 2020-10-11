# What Makes a Successful Kickstarter Campaign?

### Capstone Project for Harvard's CS50 on EdX

**Author**: Jocelyn Lutes (Boston, MA)

## Background Information
Kickstarter is an online crowdfunding platform with the mission to "help bring creative projects to life". On the platform, creators can share their ideas for projects, and backers can donate money to the cause. 

First launched in 2009, by 2018, there had already been over 300,000 campaigns launched on the site! **In this project, I will use logistic regression to predict successful vs. failed Kickstarter campaigns.**

## Methods
**Technology Used**: Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)

### Data
Data was collected from the Data Science competition site Kaggle. This data set contains data for 375,765 campaigns spanning from launch in 2009 to January 2018. Prior to use in modeling, data was cleaned to ensure no missing values and correct data types. **For this project, campaigns were only included in analysis if they were launched in the United States.**

### Exploratory Data Analysis
In order to uncover patterns and trends in the data, prior to modeling exploratory data analysis was conducted.

### Model Preparation
Prior to modeling, all categorical features were one-hot encoded, and the data was divided into training and testing sets.

### Modeling
For this project, two models were built: a baseline model and a logistic regression model. Logistic regression was chosen in order to preserve the interpretability of the model.

## Results
As shown in the table below, the logistic regression model substantially outperformed the Baseline model. The logistic regression predicted the testing data with 99.9% accuracy.

|Model|Training Score| Testing Score|
|-|-|-|
|Baseline|0.513|0.512|
|Logistic Regression|0.9995|0.9994|  

By looking at the coefficients for the logistic regression model, we are able to make recommendations about successful vs. failed campaigns.

## Recommendations
* Campaigns related to the arts seem to be more likely to find success on Kickstarter (Categories include: Film & Video, Music, Theater, Dance, Fashion, Crafts, Design, Journalism, and Photography)
* Historically, launching a campaign during the months of January or July appear to hurt your chances of having a successful campaign. On the contrary, campaigns launched in June are 2.09 times as likely to be successful!
* Campaigns launched on a Thursday, Wednesday, or Friday appear to have the most success. 
* Smaller goals do better! (Holding all else constant, as goal increases by $1, the campaign is only 0.8 times as likely to be successful. That's a reduction of 20%!).

