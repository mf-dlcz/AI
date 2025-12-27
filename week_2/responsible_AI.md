# Responsible AI
These responsible standards should be considered throughout the _entire_ lifecycle
of an AI application. This include the initial design, development, deployment, monitoring and
evaluation phases.

To operate AI responsibly, companies should proactively ensure that their systems adhere to the following
parameters:
- Fully transparent and accountable, with monitoring and oversight mechanisms in place

- Managed by a leadership team accountable for responsible AI strategies

- Developed by teams with expertise in responsible AI principles and practices

- Built following responsible AI guidelines


## Responsible AI Considerations
The rapid growth of generative AI brings promising new innovation, and at the same time, it raises new 
challenges. These include challenges that were common before generative AI, such as _bias_ and 
_explainability_. Other new challenges are unique to foundation models (FMs), such as _hallucinations_ and 
_toxicity_. 

Although the term bias is used in AI and machine learning (ML), contextually, they refer to slightly different 
matters.

**Bias in AI**  
refers to any systematic errors, unfair outcomes, or discriminatory behaviors exhibited by AI systems. 
This can include biases introduced by the training data, algorithms, or overall system design and deployment. 
Bias in AI can also manifest in various domains, such as computer vision, natural language processing (NLP), 
decision-making systems, and robotics.

**Bias in ML and DL**  
typically refers to the systematic errors or inaccuracies introduced by the learning algorithm or model 
itself. Since neural networks used in DL are also employed in generative AI systems, addressing bias at this 
level can benefit AI systems as a whole. In the context of ML and DL, bias is often discussed concerning the 
bias versus variance tradeoff, which is a fundamental concept in ML theory. Bias can arise when the model 
makes oversimplified assumptions, lacks complexity, or is trained on insufficient data.

***

### <ins>BIAS<ins>
Bias is one of the biggest challenges a developer faces in AI systems. Bias in a model means that the model is 
missing important features of datasets, which means the data is too basic. **Bias is measured by the difference 
between the expected predictions of a model and the true values we are trying to predict**. If the difference 
is narrow, then the model has low bias. If the difference is wide, then the model has a high bias. 

When a model has a high bias, it is underfitted. Underfitted means that a model is not capturing enough 
difference in the features of the data, so the model performs poorly on the training data.

### <ins>VARIANCE<ins>
Variance refers to a model's sensitivity to fluctuations or noise in the training data. The problem is that a 
model might consider noise in the data to be important in the output. When variance is high, a model becomes 
so familiar with the training data that it can make predictions with high accuracy. This is because it is 
capturing all the details in the training data.

However, when you introduce new data to the model (like test data), the model's accuracy drops. This is 
because the model has learned too much about the training data, including all the specific details and edge 
cases. As a result, the model has adapted itself closely to the training data. It cannot generalize and 
predict accurately when faced with unseen data that deviates from the training examples.

This introduces the problem of overfitting. Overfitting is when a model performs well on training data but 
does not perform well on evaluation data. This is because the model memorized the data it has seen and is 
unable to generalize for unseen examples.


## Bias Versus Variance Trade-Off
The trade-off between bias and variance is when you optimize your model with the right balance between bias 
and variance. The goal is to achieve a trained model with the lowest bias and the lowest variance trade-off 
for a given dataset. A balanced model is generalized enough to predict better when it faces unseen data. 

### UNDERFITTED
- Bias is high and the variance is low

- This leads it to conclude that the relationship between the variables is linear (represented by the 
straight line). However, the true relationship in the data follows a curved pattern.

- The regression line being a straight line indicates that the model is underfitting the data, 
failing to capture the true underlying relationships accurately.

### OVERFITTED
- Bias is low, and the variance is high

- The regression curve perfectly fits the data. This means that the model is capturing noise and essentially
memorizing the data.

- It won't perform well on new data.

### BALANCED
- Bias and variance are both low

- The regression is a curve. This is what we want.

- The model is capturing enough information in the dataset without capturing unnecessary details and noise.


## Best Practices to Overcome Bias and Variance Errors

### <ins>Cross Validate<ins>
- Cross-validation is a technique for evaluating ML models by training several ML models on subsets of the 
available input data. Then, it evaluates the models on the complementary subset of the data. You can use 
cross-validation to identify overfitting. Overfitting happens when a model performs well on training data 
but fails on new data.

### <ins>Increase Data<ins>
- To increase the learning scope of a model, you can add more data samples.

### <ins>Use Regularization<ins>
- Regularization is a method that penalizes extreme weight values to help prevent linear models from overfitting 
training data examples.

### <ins>User Simpler Models<ins>
- You could use simpler model architectures to help with overfitting. However, you should remember that 
oversimplifying a model can also lead to issues like failing to capture important patterns in the data 
(underfitting). Finding the right balance in model complexity is crucial to avoid both overfitting and 
underfitting issues.

### <ins>Apply Dimension Reduction<ins>
- Dimension reduction is an unsupervised ML algorithm that attempts to reduce the dimensionality 
(number of features) within a dataset while keeping most of the important information.

### <ins>Stop Training Early<ins>
- To ensure that a model does not memorize data, you can end training early.


## Challenges of Generative AI
Some of these challenges include regulatory violations, toxicity, intellectual property, plagiarism, hallucinations, 
and nondeterminism.

### <ins>HALLUCINATIONS<ins>
- Refer to the phenomenon where the system generates output that is inconsistent with the input data or the 
given context.

### <ins>REGULATORY VIOLATIONS<ins>
- Generative AI models trained on sensitive data might inadvertently generate an output that violates 
regulations, such as exposing personally identifiable information (PII).

### <ins>TOXICITY<ins>
- Toxicity is the possibility of generating content (text, images, or other modalities) that is offensive, 
disturbing, or inappropriate. This is a primary concern with generative AI.

- Determining what qualifies as toxic content involves subjectivity, and this presents an additional 
challenge because experts might disagree on what counts as toxic.

### <ins>INTELLECTUAL PROPERTY<ins>
- Protecting intellectual property was a problem with early large language models (LLMs). This is because 
the LLMs had a tendency to occasionally produce text or code passages that were verbatim of parts of their 
training data. This resulted in privacy and other concerns. But even improvements in this regard have not 
prevented reproductions of training content that are more ambiguous and nuanced.

### <ins>PLAGIARISM<ins>
- People worry that it could write college essays, job application samples, and enable other forms of 
cheating or copying illegally.

### <ins>Non-Determinism<ins>
- A model might generate different outputs for the same input, which can cause problems in applications 
where reliability is key.