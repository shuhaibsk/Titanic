Dataset: Titanic Dataset
Tools Used: Python, Pandas, Matplotlib, Seaborn
Objective: To analyze and extract meaningful insights from the Titanic dataset through visual and statistical exploration.

a. Data Overview
The dataset contains information about Titanic passengers, including demographics, ticket class, fare, and survival status. The data was loaded using Pandas, and initial inspection was done using .head(), .info(), .describe(), and .isnull().sum() methods.

b. Missing Value Treatment
Missing values were identified in three columns — Age, Cabin, and Embarked.
The 'Age' column had 177 missing values, which were replaced with the median age to preserve data integrity.
The 'Cabin' column had over 77% missing values and was therefore dropped.
The 'Embarked' column had two missing entries, which were filled with the most frequent value ('S').

c. Data Understanding
The 'Embarked' column represents the port where each passenger boarded the Titanic:
‘C’ stands for Cherbourg (France), ‘Q’ stands for Queenstown (Ireland), and ‘S’ stands for Southampton (England).

d. Visual Analysis and Explanations

a) Survival Count Plot:
The count plot of the 'Survived' column shows that more passengers did not survive, indicating an overall survival rate of around 38%.

b) Survival by Passenger Class:
This plot shows that first-class passengers had the highest survival rate, followed by second class, while third-class passengers had the lowest survival rate. This reflects the influence of social class on survival chances.

c) Survival by Gender:
The plot comparing 'Sex' and 'Survived' indicates that females had a much higher survival rate than males, supporting the “women and children first” policy during evacuation.

d) Age Distribution:
The histogram of 'Age' shows that most passengers were between 20 and 40 years old, with fewer elderly passengers. The distribution is slightly right-skewed, indicating fewer older individuals.

e) Boxplot of Age vs Survival:
This boxplot reveals that survivors tended to be slightly younger on average compared to non-survivors, though both groups had similar median ages.

f) Fare Distribution:
The histogram of 'Fare' shows a right-skewed distribution. Most passengers paid lower fares, but a few paid very high fares, representing first-class travelers.

g) Fare vs Survival:
The boxplot between 'Fare' and 'Survived' indicates that passengers who paid higher fares were more likely to survive. This suggests that wealthier passengers (mostly first-class) had better survival chances.

h) Correlation Heatmap:
The heatmap shows relationships between numerical variables. 'Fare' and 'Pclass' show a strong negative correlation (higher fares are linked to first-class tickets). 'Survived' is moderately correlated with 'Fare' and weakly correlated with 'Age' and 'Pclass'.

i) Pairplot (Age, Fare, Survived):
This visualization displays pairwise relationships between Age and Fare, colored by survival status. Survivors tend to cluster around higher fares and lower ages, especially in first-class sections.

j) Survival by Embarked Port:
This bar plot shows that passengers who boarded from Cherbourg (C) had the highest survival rate, while those from Southampton (S) had the lowest. This is likely because more first-class passengers boarded at Cherbourg.

e. Key Findings
a. Females had a much higher survival rate compared to males.
b. First-class passengers had the best chances of survival, showing the impact of social class.
c. Higher fares were associated with better survival outcomes.
d. Passengers boarding from Cherbourg had better survival rates.
e. Younger passengers and those with small families were more likely to survive.

f. Conclusion
The Titanic dataset clearly reflects the social and demographic inequalities that affected survival chances. Gender, class, fare, and embarkation point were the strongest predictors of survival. After handling missing values and visualizing the data, it was evident that socioeconomic status and access to lifeboats played a crucial role in determining who survived the tragedy.
