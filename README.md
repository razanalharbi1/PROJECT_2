# Disaster Response Pipeline Project
This project is to classify disaster response messages through machine learning.
# Project Components

1. ETL Pipeline
The ETL script, etl_pipeline.py takes the file paths of the two datasets and database, cleans the datasets, and stores the clean data into a SQLite database in the specified database file path.

2. ML Pipeline
The machine learning script, train_classifier.py takes the database file path and model file path, creates and Builds a text processing and machine learning pipeline, trains a classifier and tunes a model using GridSearchCV, and stores the classifier into a pickle file to the specified model file path.

3. Flask Web App
The web app includes two visualizations using data from the SQLite database.

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

# screenshots 

![2021-12-30 (5)](https://user-images.githubusercontent.com/93232920/147765062-fbce1f82-aa46-4cb1-ba78-f01a19b03683.png)

![2021-12-27 (2)](https://user-images.githubusercontent.com/93232920/147765082-1e57d5e9-b8ba-486e-96c2-11e03511b296.png)

![2021-12-30 (6)](https://user-images.githubusercontent.com/93232920/147765066-f10810a3-c0ea-4fdb-b27d-7c195de80abd.png)


# Credits and Acknowledgements

Thanks Udacity
