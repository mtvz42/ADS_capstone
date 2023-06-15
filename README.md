# SpaceX Falcon 9 first stage landing prediction

This project aims to predict whether the SpaceX Falcon 9 first stage will land successfully.
SpaceX advertises Falcon 9 rocket launches on their website at $62 million; other providers cost upwards of $165 million per launch, with much of the savings coming from SpaceX's ability to reuse the first stage.
Therefore, if we can determine whether the first stage will land, we can determine the cost of a launch.
This information can be used if an alternative company wants to bid against SpaceX for a rocket launch.

## Part 1: Data Collection using Web Scraping
In this part, web scraping is done using Python BeautifulSoup package, to collect Falcon 9 historical launch records from a Wikipedia page titled 'List of Falcon 9 and Falcon Heavy launches'
https://en.wikipedia.org/wiki/List_of_Falcon\_9\_and_Falcon_Heavy_launches
Notebook file: 1_1_Data_collection_API.ipynb

Part 2: Data Collection using SpaceX API
In this part, data is collected from the SpaceX API. Basic data wrangling and formatting is done.
Notebook file: 1_2_Data_collection_web-scraping.ipynb

Part 3: Data Wrangling
In this part, Exploratory Data Analysis (EDA) is performed to find some patterns in the data and determine what would be the labels for training supervised models.
Notebook file: 1_3_Data_collection_data-wrangling.ipynb

Part 4: Exploratory Data Analysis with SQL
In this part, the Spacex Dataset is loaded into a corresponding table in a Db2 database and SQL queries are executed to better understand the data.
Notebook file: 2_1_EDA_with_SQL.ipynb

Part 5: Exploratory Data Analysis with Visualization
In this part, exploratory data analysis and Feature Engineering is performed using Pandas and Matplotlib.
Notebook file: 2_2_EDA_with_visualizations.ipynb

Part 6: Data Visualization using Folium
In this part, more interactive visual analytics are performed using Python Folium package.
Notebook file: 3_1_Interactive_visual_analytics_with_Folium.ipynb

Part 7: Plotly Dashboard
In this part, an interactive dashboard app is created based on the SpaceX dataset, using Python Dash and Plotly packages.
Script file: 3_2_Interactive_dashboard_with_Ploty_Dash.py

Part 8: SpaceX Machine Learning Prediction
In this part, data is analysed, split into training and testing sets and 4 supervised models- Support Vector Machine, Decision Tree, K-Nearest Neighbours and Logistic Regression, are trained on the dataset. The accuracy of each of the models is calculated to find the best prediction model.
Notebook file: 4_1_Machine_Learning_prediction.ipynb
