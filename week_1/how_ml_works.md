# How Machine Learning Works
- ML develops algorithms and statistical models.

- ML models find patterns and relationships in data, and they don't rely on hard-coded
rules or instructions.

## Difference between Machine Learning and classical programming
- Machine Learning involves teaching a computer to recognize patterns by example, rather than
programming it with specific rules.

- ML, is about creating algorithms (or sets of rules).

- These algorithms learn from complex functions (patterns) in data.

- With ML, you start with a problem, identify data associated with the problem, use an algorithm
to model the problem, and then generate output.


## Machine Learning Application Development Process
Building ML applications is an iterative process that involves

1. **Formulate a Problem**
    - Define the problem that you're trying to solve and the goal that you want to reach.
    - Frame the core ML problem in terms of what is observed and what answer you want the model
    to predict.

2. **Prepare your Data**
    - You collect, clean, and prepare data to make it suitable for ML model training algorithms.
    - Visualize and analyze the data, and run sanity checks to validate the quality of the data
    and understand it.

3. **Train the Model**
    - To train a highly predictive model, the raw data and answers can't always be used effectively.
    - Preferably, construct more predictive input representations or features from the raw variables.
    - Feed the resulting features to the learning algorithm to build models.
    - Set aside a subset of the input data to test the model.

4. **Test the Model**
    - Evaluate the quality of the models using data that was held out from model building.

5. **Deploy your Model**
    - Use the model to generate predictions of the target answer for new data instances.

<br>

## Building a Machine Learning Model
- Building a machine learning model involves
1. data collection & preparation
2. selecting an appropriate algorithm
3. training the model on the prepared data
4. evaluating its performance through testing and iteration

### Training Data
- The machine learning process begins with gathering and preparing data.

- Poor quality data is often referred to as _garbage in, garbage out_ (GIGO).

- Although data preparation may seem routine, it is arguably the most important step in ensuring
a model works as intended.

- **_Labeled Data_** has been tagged or classified while **_unlabeled data_** has not been categorized.

- Many ML algorithms require labeled data, where the model is trained on examples with known outputs
or labels.

- Other algorithms can work with _**unlabeled data**_ to find patterns or structure within the data.

    ### Labeled Data
    - **_Labeled Data_** is a dataset with labels or target variables.
    
    - These labels show the desired output or classification.

    - Labeled data sometimes is called _ground truth_ among ML practitioners.

    **EXAMPLE:**  
        - labeled data has images and their class labels.  
        - For example, an image may be labeled as cat, dog, or car
