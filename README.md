
## Disaster Response Pipeline Project 

### Table of contents
1. Porject Overview
2. Project Structure
3. Installation
4. Instruction
5. Acknowledgements
6. License

#### Project Overview
This project is part of the Udacity Data Scientist Nanodegree program. The goal of this project is to build a web application that can classify disaster-related messages into different categories, allowing for effective response and aid coordination during emergencies.

#### Project Structure
- app/: Contains the Flask web application files.
	- templates/: HTML templates for the web application.
    - run.py: Script to run the web application.
- data/: Contains the disaster response dataset and the ETL pipeline script.
	- disaster_messages.csv: Input dataset containing disaster-related messages.
    - disaster_categories.csv: Input dataset containing message categories.
    - process_data.py: ETL pipeline script for data cleaning and preprocessing.
    - DisasterResponse.db: SQLite database to store the cleaned data.
- models/: Contains the ML pipeline script and the trained model.
	- train_classifier.py: ML pipeline script for training the classification model.
	- classifier.pkl: Trained machine learning model saved as a pickle file.
- README.md: Project overview and instructions.

#### Installation
You won't need any additional libraries apart from the ones that come with the Anaconda distribution.

#### Instruction
1. Run the following commands in the project's root directory to set up your database and model.
	- To run ETL pipeline that cleans data and stores in database 
    python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db
	- To run ML pipeline that trains classifier and saves 
    python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl
2. Run the following command in the app's directory to run your web app. python run.py
3. Go to http://0.0.0.0:3001/
#### Acknowledgements
- This project is based on the Disaster Response Messages dataset provided by Figure Eight.
- Special thanks to Udacity for providing the project idea, guidance, and necessary resources.
#### License
- This project is licensed under the MIT License.


