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


## Responsible AI considerations
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


## Bias versus variance trade-off
