
# Winning Space Race with Data Science

## Table of Contents
1. Overview
2. Methodology
    - Data Collection
    - Data Wrangling
    - Exploratory Data Analysis (EDA)
    - Interactive Visual Analytics
    - Predictive Analysis
3. Key Findings
    - Exploratory Data Analysis (EDA)
    - Interactive Analytics
    - Predictive Analysis
    - Conclusion
4. Limitations of the Study
5. Project's Impact
6. Project's Challenges
7. Appendix
8. References

## Overview
This project, part of the IBM Applied Data Science Capstone, focuses on predicting the cost of a SpaceX launch based on reusability using public data on past launches and machine learning techniques. By leveraging SpaceX's reusability as the key factor, the model aims to predict launch costs accurately.

## Methodology

### Data Collection
- **API Requests**: We gathered SpaceX's past launch data via their open-source API. The data was retrieved using GET requests and processed to include only Falcon 9 launches. Missing payload weights from secret missions were filled with average values. The API provided comprehensive details on each launch, including flight number, payload mass, launch site, orbit type, and mission outcome.
- **Web Scraping**: Historical Falcon 9 and Falcon Heavy launch data were extracted from Wikipedia using BeautifulSoup. The HTML content was parsed, and the relevant table data was transformed into a Pandas DataFrame. The web scraping process involved requesting the webpage's HTML content, parsing the relevant table, and extracting column names. The data from each table row was stored in a dictionary, which was subsequently transformed into a Pandas DataFrame.

### Data Wrangling
- **Data Cleaning**: The collected data underwent a cleaning process to organize and standardize it for subsequent analysis. This included handling missing values, converting data types, and ensuring consistency in formatting.
- **Label Creation**: A binary label representing successful or unsuccessful landings was created to train machine learning models.

### Exploratory Data Analysis (EDA)
- **Data Visualization**: Various charts were plotted to visualize relationships between flight number, payload mass, launch site, orbit type, and success rates.
- **SQL Queries**: Unique launch sites, payload mass calculations, and mission outcomes were analyzed using SQL queries.

### Interactive Visual Analytics
- **Folium Maps**: Interactive maps were created to visualize launch site distribution and success rates. Circles, markers, and clusters were used to enhance visualization.
- **Plotly Dash**: Dashboards with pie charts and scatter plots were built to enable dynamic exploration of data.

### Predictive Analysis
- **Model Building**: Multiple classification models were constructed, including Logistic Regression, Support Vector Machine (SVM), Decision Tree, and K-Nearest Neighbors (KNN).
- **Hyperparameter Tuning**: GridSearchCV was employed for hyperparameter tuning to optimize model performance.
- **Model Evaluation**: Models were evaluated based on accuracy and confusion matrices. SVM emerged as the top-performing model.

## Key Findings

### Exploratory Data Analysis (EDA)
- **Flight Experience**: The success rate of SpaceX launches generally increased from 2013 to 2020, indicating improvements in technology and processes.
- **Payload Mass**: Heavier payloads tend to have a slightly lower success rate, especially for certain orbit types.
- **Launch Site**: Different launch sites exhibit varying success rates, suggesting that site-specific factors could play a role.
- **Orbit Type**: Certain orbits (ES-L1, GEO, HEO, SSO) show a 100% success rate, while others (GTO, SO) have more variability.
- **Booster Version**: The choice of booster version might also influence the success rate, with newer versions potentially performing better.

### Interactive Analytics
- **Dynamic Exploration**: Interactive analytics empowers users to explore and analyze data dynamically, uncovering insights, identifying trends, and making data-driven decisions quickly.

### Predictive Analysis
- **Top Performing Models**: SVM, Logistic Regression, and Decision Tree models emerged as the top performers in predicting launch success.
- **Potential for Improvement**: Further analysis is needed to definitively select the best model among the top three, considering factors like interpretability, complexity, and training time.
- **Confusion Matrices**: Confusion matrices provide valuable insights into model predictions, highlighting areas where the model excels or struggles.

### Conclusion
The analysis successfully identified key factors that may influence the success of SpaceX launches, including payload mass, launch site, orbit type, and booster version. The machine learning models developed can be valuable tools for predicting launch success and optimizing mission parameters.

## Limitations of the Study
- **Data Quality**: The accuracy of the analysis is dependent on the quality of the data collected. Any errors or inconsistencies in the data could impact the results.
- **Sample Size**: The study is limited by the sample size of the data. A larger dataset could provide more robust and reliable results.
- **Model Assumptions**: The predictive models are based on certain assumptions that may not hold true in all scenarios. These assumptions could affect the accuracy of the predictions.
- **External Factors**: The study does not account for external factors such as weather conditions, geopolitical events, or technological advancements that could influence launch success.
- **Generalizability**: The findings may not be generalizable to other space missions or companies, as the study focuses specifically on SpaceX launches.

## Project's Impact
The project's impact is multifaceted, contributing to both the scientific community and the broader space industry:
- **Cost Efficiency**: By accurately predicting launch costs based on reusability, the project helps SpaceX and other space companies optimize their budgets and reduce expenses.
- **Mission Planning**: The insights gained from the analysis can inform mission planning, enabling more efficient allocation of resources and better decision-making.
- **Technological Advancements**: The project highlights the importance of technological advancements in improving launch success rates, encouraging further innovation in the space industry.
- **Environmental Benefits**: Reusable rockets contribute to sustainability by reducing waste and minimizing the environmental impact of space missions.
- **Educational Value**: The project serves as a valuable educational resource for students and researchers interested in data science, machine learning, and space exploration.

## Project's Challenges
The project faced several challenges that impacted its execution and outcomes:
- **Data Availability**: Access to comprehensive and up-to-date data was a significant challenge. Some data points were missing or incomplete, requiring imputation and assumptions.
- **Data Integration**: Combining data from multiple sources (API, web scraping) posed challenges in ensuring consistency and accuracy.
- **Feature Engineering**: Identifying and creating relevant features for the predictive models required extensive domain knowledge and experimentation.
- **Model Complexity**: Balancing model complexity with interpretability was a challenge, as more complex models often provided better accuracy but were harder to interpret.
- **Computational Resources**: Training and tuning multiple machine learning models required significant computational resources and time.
- **External Validation**: Validating the models with external data or real-world scenarios was challenging due to the lack of publicly available data on recent launches.

## Appendix
Include relevant assets like Python code snippets, SQL queries, charts, Notebook outputs, or data sets created during this project.

## References
: SpaceX API
: Wikipedia
: Data Cleaning
: Label Creation
: Data Visualization
: Data Visualization
: SQL Queries
: SQL Queries
: Folium Maps
: Model Building
: Model Evaluation


