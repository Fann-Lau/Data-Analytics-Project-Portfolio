# Data-Analytics-Project-Portfolio
My Data Analytics Project Portfolio 
Application of Python in Analyzing Telephone Fraud Activities
# Overview
This project leverages various Python libraries and machine learning techniques to analyze the relationship between economic characteristics and telephone fraud activities while attempting to predict the themes and frequency of such fraud. The primary goal of this study is to understand the patterns of telephone fraud and provide support for developing targeted prevention strategies.
# Data Collection and Cleaning
I utilized the pandas library to load data from multiple sources, including telephone fraud data from the Federal Trade Commission (FTC), economic data from the Bureau of Economic Analysis (BEA), and state-level education data published by the National Center for Education Statistics (NCES). The cleaning process involved removing duplicates, handling missing values, and renaming columns to ensure data consistency. Subsequently, these datasets were merged using a shared variable, "State," to create a unified dataset for further analysis and modeling.
# Data Exploration and Statistical Analysis
Using pandas and scipy.stats, I conducted an in-depth analysis of the relationship between economic characteristics and telephone fraud activities. Descriptive statistics and Pearson correlation coefficients revealed a significant positive correlation between population size and the number of reported fraud calls, while the correlation between per capita income and fraud activities was weaker. Furthermore, different types of fraud (e.g., energy-related fraud vs. medical fraud) showed distinct state-level distribution patterns. For better visualization, I used seaborn and matplotlib to generate correlation heatmaps and distribution plots.
# Feature Engineering and Modeling
During the modeling phase, I expanded the range of economic variables to include per capita GDP, personal income, regional price parity, employment numbers, and state-level educational statistics. To address scale differences among features, I applied standardization using sklearn.preprocessing.
I employed multiple machine learning models, including linear regression, Lasso regression, random forest, gradient boosting, and neural networks (via tensorflow.keras). Model performance was evaluated using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R² scores. Among these, the Lasso model demonstrated the best stability and generalization ability, making it particularly suitable for predicting the themes and frequencies of telephone fraud activities.
# Conclusions
The project findings indicate a significant relationship between economic characteristics and telephone fraud activities. Total income and population size were identified as key drivers of fraud activity, while per capita income had a relatively minor impact. Additionally, the state-level distribution of different types of fraud varied significantly with economic characteristics. Building predictive models enables tailored preventive measures for specific regions.
# Limitations and Future Directions
This study is subject to several limitations:
The data covers a specific time period and region, which may not fully represent nationwide fraud activities.
The analysis focuses on economic characteristics (e.g., income, population) while excluding other potential factors like social, cultural, or technological influences.
Fraud strategies evolve over time, necessitating continuous data updates to maintain model relevance.
Future research can address these limitations by:
Expanding the scope of the dataset to include broader time periods and regions.
Incorporating additional dimensions such as societal, cultural, and policy-related data for a more comprehensive analysis.
Continuously tracking and updating data to adapt to dynamic changes in fraud patterns.

# Python's Role in This Project
This project exemplifies Python’s ability to provide an end-to-end solution for complex data analysis and problem-solving. From data preprocessing to machine learning modeling, Python’s powerful libraries—such as pandas, scipy.stats, sklearn, and tensorflow.keras—played a crucial role in delivering actionable insights and predictive capabilities for addressing telephone fraud activities.
