# Disaster Response Pipeline Project

## Project Description:
In this project, a data transformation - machine learning pipeline is developed that is capable to curate the class of the messages. It is deployed in a flask application. The project include a web app where an emergency worker can input a new message and get classification results in several categories. The landing page of the webapp also includes 4 visualizations of the training dataset built with plotly.

File Descriptions:
The project contains the following files,

- ETL Pipeline Preparation.ipynb: Notebook experiment for the ETL pipelines
- ML Pipeline Preparation.ipynb: Notebook experiment for the machine learning pipelines
- data/process_data.py: The ETL pipeline used to process data in preparation for model building.
- models/train_classifier.py: The Machine Learning pipeline used to fit, tune, evaluate, and export the model to a Python pickle 
- app/templates/~.html: HTML pages for the web app.
- run.py: Start the Python server for the web app and prepare visualizations.
 

Example message to classify: "Help, Robber!"

### Local Instructions:
Run the following commands in the project's root directory to set up your database and model.

 - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
 - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

Go to http://0.0.0.0:3001/
#### Application looks like below: 

![image](https://drive.google.com/uc?export=view&id=1913oZeBZPBNiUuk8gu3ZSbLBA2l_VQtG)
