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

    ### Unlabeled Data
    - **_Unlabeled Data_** is a dataset where the instances (data points) or examples do not have
    any associated labels or target variables.

    - The data consists only of input features, without any corresponding output or classification.

    **EXAMPLE**  
        - In image classification, unlabeled data is a collection of images without any labels or 
        annotations.
    
<br>

***
### Structured Data
- Structured Data is organized and formatted in a specific way, usually in tables or databases with
rows and columns.

- This type of data works well with traditional machine learning algorithms that require clear features
and labels.

Structured Data includes the following:
- **Tabular Data**: This includes data stored in spreadsheets, databases, or .csv files.
    - The rows represent individual instances, and the columns represent features or attributes.

- **Time-series Data**: Thi type of data consists of a sequence of values measured at different
points in time, such as stock prices, sensors readings, or weather data.

### Unstructured Data
- Unstructured Data is information without a specific format.

- It includes text, images, audio, and video.

- It's extremely hard (if possible) to use traditional machine learning models to find patterns in
unstructured data.

Unstructured Data includes the following:
- **Text Data** This type of data includes documents, articles, and social media posts.
    - It also includes other forms of written content.

- **Image Data** This data category covers digital images and photographs.
    - It also includes individual frames from videos.

<br>

<br>

## Machine Learning Process
- In the machine learning process, the compiled trained data is fed into machine learning
algorithms.

- This process is traditionally divided into three broad categories - supervised learning,
unsupervised learning, and reinforcement learning.

### Supervised Learning
- Algorithms are trained on _labeled data_.

- The goal _is to learn a mapping function that can predict the output for new, unseen input
data_.

- In supervised learning (in this case, a human) provides labeled training data.
Like a student, a supervised algorithm learns by example.

- This type of algorithm uses the training data to determine the patterns and relationships
between the inputs and outputs.

Depending on the target feature being predicted, supervised learning has the two following subcategories-classification and regression.

#### _Classification_
Is a supervised learning technique used to assign labels or categories to new, unseen data instances based on a trained model.

- The model is trained on a labeled dataset, where each instance is already assigned to a known class or category.

- The goal of classification is to **learn patterns from the training data and use them to predict the class or category
for new unlabeled data instances**.



### Unsupervised Learning


### Reinforcement Learning
