# Customers-Segmentation-Unsupervised-ML-project-in-Python

### Problem Statement:
  - understand the target customers to plan a marketing strategy.
  - identify the most important shopping groups based on annual income, age, gender, and their shopping score.
  - identify the ideal number of groups and labeling them using the Elbow's method.

<br/>


### Project approach:
  - EDA (Exploratory Data Analysis)
  - Utitlize KMeans clustering algorithm
  - from the created clusters use Summary Statistics

<br/>


# EDA (Exploratory Data Analysis)

## 1. Univariate Analysis: to describe and summarize the distribution of a single variable

#### ***I) looking at distributions of each column***
![image](https://github.com/user-attachments/assets/66e69ff6-880f-45d5-9381-e2a93a054ed2)
1. Distribution of Age:
  - it's roughly distributed with a peak for people aged around 30-50 years.
  - There're also some slightly peaks around 20 and 40 years, indicating other age clusters

2. Distribution of Annual Income (in $k):
  - The income is right skewed where few people has higher annual income.

3. Distribution of spending score:
  - The distribution is relatively uniform, where most customers have a moderate spending habits.

  >**I recommend**: 
  > *Marketing strategies could target the 30-35 age group, as they are the most common customers. Also, High-income individuals (80k+) might be valuable for premium services.*

<br/><br/>

#### ***II) looking at distribution of each column Vs. Gender***

![image](https://github.com/user-attachments/assets/ff518824-e702-4d60-b533-077cd6c5f924)
- we can see clearly that 'Females' portion is more frequent than that of 'Males'.
- Also there is an outlier in the 'Male' as it has a right thick tail with the distribution skewed to the right.
  - So to investigate this outlier:
    
  ![image](https://github.com/user-attachments/assets/92bf15c8-44ee-436a-8e2b-29bd4a6b3c98)

  > **Interpretation:**
  > - The median income for females appears slightly lower than that for males.
  >  - There’s one outlier among males, indicating a significantly higher income.


<br/>

## 2. Bivariate Analysis:

#### I) understanding customers behavior based on demographic factors like age and gender in relation to income and spending habits. 
![image](https://github.com/user-attachments/assets/1623fb91-564c-488d-9c7b-945389a0f392)

- In 'Annual Income vs. Spending Score':
  - There may be a pattern found related to annual income and spending score
- In 'Age vs. Spending Score':
  - No strong correlation wes found.
  - Younger individuals may have slightly higher spending scores.
- In 'Age vs. Annual Income' :
  - No correlation was found
  - Income is different across all age groups

#### II) identify relationships between variables:
![image](https://github.com/user-attachments/assets/680eb388-5100-435d-9f57-12201a495113)

- In 'Age vs. Spending Score' :
  - There is a strong negative correlation (-0.33) between age and spending score.
  - Younger individuals tend to have higher spending scores.
- There's no clear correlation between 'Annual Income' and 'Spending Score'
- There's almost no correlation between 'Age' and 'Annual Income'

<br/><hr/><br/>

# Using K-means clustering ML algorithm, I found:
![image](https://github.com/user-attachments/assets/593f46f8-b37f-49a8-865f-fc9362012afd)

#### Trends & Patterns found:
1. target cluster would be cluster 1 which has a high spending score and high annual income.
2. approxiamtley 54% of females in cluster 1 shoppers are females. we should look for ways to attract more of them using a marketing campaign targeting popular items in this cluster.
3. cluster 4 has a potential in sales. so we should make an event on popular items purchased by them.
