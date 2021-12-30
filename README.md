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

# Credits and Acknowledgements

Thanks Udacity
