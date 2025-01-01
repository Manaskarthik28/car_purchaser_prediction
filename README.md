# 1. Uploading Raw Car Purchase Data to Azure Blob Storage
I first uploaded the raw car purchase data into my Azure Blob Storage account.
The data was stored in a container called rawdata.
The dataset contains the following columns:
User_ID: A unique identifier for each user.
Gender: Gender of the user.
Average_Salary: The user's average salary.
Purchased: A binary indicator where 0 represents a purchase (Yes) and 1 represents no purchase (No).
# 2. Data Transformation in Databricks
To clean the raw data, I connected the rawdata container to Azure Databricks.
I performed the following transformations:
Removed null values to ensure the dataset was clean and free from incomplete data.
Dropped irrelevant columns that were not necessary for the analysis.
The cleaned dataset was then saved into a new container named cleandata in Azure Blob Storage.
# 3. Data Processing and AutoML in Azure ML Studio
After preparing the cleaned data, I connected the cleandata container to Azure Machine Learning Studio.
I used AutoML in Azure ML Studio to perform a Logistic Regression model, as the task was a classification problem.
The dataset was used to predict whether a user would purchase based on the Gender and Average_Salary columns.
The logistic regression model achieved an 85% accuracy in predicting car purchases.
# 4. Visualization in Power BI
After the model training, I connected the processed data and results to Power BI for visualization.
Using Power BI, I created a dashboard to visualize the insights derived from the cleaned and processed data.
The dashboard showcased the purchase predictions and included insights from the logistic regression model, such as trends and patterns in Gender and Average_Salary that influenced the likelihood of purchasing.
