# 1. Uploading Raw Car Purchase Data to Azure Blob Storage
I first uploaded the raw car purchase data into my Azure Blob Storage account.
The data was stored in a container called rawdata.
This raw dataset contained several columns, some of which were irrelevant or contained missing values.
# 2. Data Transformation in Databricks
To clean the raw data, I connected the rawdata container to Azure Databricks.
I performed the following transformations:
Removed null values to ensure the dataset was clean and free from incomplete data.
Dropped irrelevant columns that were not necessary for the analysis.
The cleaned dataset was then saved into a new container named cleandata in Azure Blob Storage.
# 3. Data Processing and AutoML in Azure ML Studio
After preparing the cleaned data, I connected the cleandata container to Azure Machine Learning Studio.
I used AutoML in Azure ML Studio to perform a Logistic Regression model since the task was a classification problem.
After running the AutoML process, the logistic regression model achieved an 85% accuracy on the dataset.
# 4. Visualization in Power BI
After the model training, I connected the processed data and results to Power BI for visualization.
Using Power BI, I created a dashboard to visualize the insights derived from the cleaned and processed data.
The dashboard provided a comprehensive view of the car purchase predictions, showcasing the results of the logistic regression model, along with any additional insights relevant to the analysis.
