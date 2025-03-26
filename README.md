# Quantitative Data-Analysis
Bait Lamina App (Feedback Analysis)

Closed-ended Questions (quantitative): These questions helped to measure the overall usability of the app and identify the key drivers of satisfaction. Most of the questions used a Likert scale from 1 to 5, where 1 is considered as high and 5 as low. Similarly, the questions also included binary and multiple-choice options. These questions cover several aspects of the app and user experience: 

Understanding of the Bait Lamina Method: After engaging with the web app, students were asked to rate their understanding of the method from 1 to 5. 

Ease of Navigation and Use: Students were asked to evaluate and rate the navigation and ease of use (1 to 5). 

Clarity of the Calculation Process: Students were asked to rate the clarity of the calculation process in the app (1 to 5). 

Scatter Plot Evaluation: Students were asked to rate the usefulness of the scatter plot feature for visualization (1 to 5). 

Automated Report Generation: Students were asked if they found the reporting feature useful (yes or no). 

Overall Satisfaction: Students were asked to rate their overall satisfaction with the app (1 to 5). 

Comparison with Excel: Students were offered a multiple-choice question on a five-point scale, ranging from "strongly agree," "somewhat agree," "neutral," "somewhat disagree," and "strongly disagree," to indicate their agreement with the statement that online apps outperform Excel for equivalent activities. 

#  Quantitative Analysis  

Quantitative analysis was used to analyze patterns, correlations, and significance in relationships between different variables. The study included a variety of statistical methods to analyze user perception and assessment of the app in a variety of areas, including technique comprehension, ease of navigation and usage, clarity, feature utility, and overall satisfaction.   

Python libraries such as Pandas, NumPy, Phi-k, SciPy, and Stats models were utilized in the analysis, while Matplotlib and Seaborn were used for visualization. The essential libraries were imported to analyze data distribution and perform phi coefficient (φK) correlation, OLS regression, and chi-square testing. Finally, after successfully importing the libraries, the dataset was imported for analysis. 

1 Exploratory Data Analysis 
Exploratory Data Analysis (EDA) was conducted to understand the underlying structure of the data and identify patterns, anomalies, or trends. The distribution of student feedback across various usability aspects was explored using bar diagrams, and the results were further analyzed. 

2 Data Preprocessing 
The data were converted from categorical to numerical format to ensure they all had the same scale to conduct multiple OLS regression. Likewise, to achieve consistent scale, the ordinal categorical data were converted to numerical values using mapping dictionaries. The student's responses were converted from qualitative options (e.g., 'Quite clear,' 'Neutral,' 'Quite puzzling') to numerical values ranging from 1 to 5 ('Quite clear' was mapped to 1, and 'Quite confusing' to 5). Furthermore, user preferences for utilizing the web app over Excel were mirrored in two additional comments from users who identified as others, where positive and neutral suggestions were encoded as 1 and 3, respectively.

3 Phi Coefficient Correlation Analysis 
The Phi coefficient (φK) correlation analysis was employed to identify the correlation between the categorical and continuous variables. This approach generalizes the chi-square test and adapts it to provide more meaningful correlation results, making it more versatile for mixed datasets. It involves reclassification of continuous variables into categorical formal, known as bins, and applying an adapted version of the Pearson correlation, generalized to handle non-linear relationships. Once all the variables are converted into categories, the values are normalized into the scale between 0 and 1 to ensure comparability. It calculates the correlation between two binary variables and is frequently used to evaluate the degree of connection between various variables in contingency tables, particularly 2x2 tables. This approach was useful in finding the correlation between the usability aspects of the app and user demographics. The dataset included categorical variables such as 'usefulness of report generation' (with 'yes' or 'no' responses), 'gender,' and 'student level'. The libraries used for the analysis are Phik and visualization was created in a heatmap using Seaborn. 

4 Chi-square Test 
The Chi-square test of independence, often known as the Pearson Chi-square test, is an effective statistical tool for evaluating concepts using nominal or ordinal variables. It was utilized to identify the association between various categorical variables. Several chi-square tests were used to analyze the relationship and significance of categorical variables, such as report generation usefulness vs. overall satisfaction and student vs. method understanding. Similarly, this study influenced the app's design decisions by identifying areas where user demographics significantly impact usability perceptions. Such insights can help guide targeted upgrades, ensuring that capabilities align better with user expectations across categories. SciPy and Seaborn libraries are used for data processing and visualization. 

5 Multiple OLS Regression Analysis 
Multiple OLS regression analysis is a statistical approach that examines the relationship between numerous linear variables. These variables are often called dependent and numerous independent variables. To separate the distinctive influences of each independent variable from the dependent variable, their contribution is evaluated while keeping others constant. OLS regression, a prominent multiple regression analysis approach, was used to discover important drivers of overall satisfaction. Understandability, clarity, ease of navigation and use, feature usefulness, and user preferences were considered independent variables, whereas overall satisfaction was dependent. The Statmodel library was used to conduct the analysis, and Matplotlib was used to visualize the results. 
