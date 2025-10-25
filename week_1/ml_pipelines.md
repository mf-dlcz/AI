# ML Pipelines
- A machine learning pipeline is a series of steps that work together to perform a machine 
learning task.

- Engineers design the pipeline to automatically do the different parts of creating a machine 
learning model.

- The pipeline takes in and prepares data.
    - It then trains the model on the processed data and evaluates how well the model
    performs.
    - It also deploys the trained model so that others can use it.

****
A typical machine learning pipeline includes the following stages:

### Problem Formulation
- Is an essential initial step that involved clearly defining and understanding the problem to be
addressed.

- This stage identifies the learning problem type (supervised, unsupervised, or reinforcement).

- It also determines the evaluation criteria, establishes data requirements, and identifies
constraints and assumptions.

- It provides a clear direction for data collection, preprocessing, model selection and evaluation.

- A well-formulated problem ensures that the machine learning solution aligns with business goals.
    - It also ensures that appropriate techniques and resources are used effectively.


### Data Gathering and Ingestion
- In this stage you upload and import data from various sources.

- These sources can include databases, CSV files or APIs.

- Data is brought into the machine learning environment for further processing.


### Data Preprocessing
- The data processing stage involves cleaning and transforming the raw data.

- This step ensures that the data is in a format suitable for machine learning algorithms.

- It might include handling missing values, encoding categorical variables, scaling numerical
features, and splitting the data into training and testing sets.

- Often, data preprocessing and the next stage, feature engineering, can be done at the same
time.

<br>

***
## <center> Model Tuning <center/>

### Feature Engineering
- Is the process of creating new features from existing ones.

- This stage helps ML algorithms better represent patterns in the data.

- It involves the following three techniques:
1. **Feature Selection** This selects the most relevant features from the existing set of features.

2. **Feature Extraction** This creates new features by combining or transforming existing features. 
    - For example, you can transform a date into separate numerical columns for month, day and year.

3. **Feature Construction** This generates new features based on domain knowledge or expert insights.
    - For example, if you have data on an individual's weight and height, you could construct a 
    new feature.


### Model Selection and Training
- In the model selection and training stage, you choose an ML algorithm that suits your problem and
data (for example, classification or regression).

- Different algorithms have different strengths and weaknesses.

- Selecting the right algorithm is crucial for good performance.

- You then train the selected model on the preprocessed data by using the chosen algorithm.

- During training, the algorithm learns patterns and relationships from the data.

- The goal is to find the best model that can make accurate predictions on new, unseen data.


### Model Evaluation
- Involves assessing the trained model's performance using metrics like accuracy, precision, and
recall.

- This evaluation is done on a held out test set or through cross-validation.


### Content with Performance
_**Yes**_

### Model Deployment
- After the model performs well, you can deploy it to the next higher environment, whether it's a 
production or non-production environment.

### Monitoring
- Finally, you monitor the model's performance after deployment.

- After a while, a model's performance might degrade, which is identified through continuous monitoring.

- The process of monitoring, updating and upgrading a model to a better version is known as machine
learning operations (MLOps).

- MLOps also involves retraining the model as needed to adapt to changing data patterns, keeping the model
accurate and reliable in real-world use.

_**No**_

### Model Tuning
- All of the steps within Model Tuning will repeat.

<br>

*****

CONTENT WITH PERFORMANCE:
|        Yes        |      No      |
|-------------------|--------------|
| Model Deployment  |  Model Tuning|
|     Monitoring    |  Repeats the model tuning process  |