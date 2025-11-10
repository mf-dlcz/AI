# Deep Learning Fundamentals
- The field of deep learning (DL) is inspired by the structure and function of the brain. 

- Deep learning involves the use of artificial neural networks, which are computational 
models that are designed to mimic the way the human brain processes information.

- DL has emerged as a powerful technique for solving complex problems that traditional 
ML algorithms often struggle with.

- Unlike traditional ML algorithms, deep learning algorithms can automatically learn hierarchical 
representations from raw data.

- Hierarchical representations emerge because deep neural networks have multiple layers of neurons.

- **The initial layers learn low-level features**, like edges or simple patterns, directly from the 
raw input (for example, pixels in images). Subsequent higher layers then combine the low-level 
features into more abstract, higher-level representations that capture more complex concepts.


## Neural Networks
- Deep learning is based on neural networks.

- Just like our brains have biological neurons that are connected, neural networks have many small 
units, called nodes, connected together.

- These nodes are organized into layers. The layers include an **input layer, one or more hidden 
layers, and an output layer**.

- When you show a neural network many examples, it will figure out how to identify patterns. 
It does this by adjusting the connections' weights between its nodes. 

- As the neural network learns from the data, it develops internal representations of the input in 
its hidden layers. These internal representations are referred to as latent representations 
(or latent space).

- Latent representations are the compressed, low-dimensional representations of the input data 
learned by a neural network model.

- Latent representations are the compressed, low-dimensional representations of the input data 
learned by a neural network model.

- **Latent representations are useful for tasks like dimensionality reduction, data compression, 
and generating new data instances**.

- In some cases, you might want to find the probability distribution of the latent representations 
(or latent variables) that could have generated the observed data. However, calculating this 
probability distribution directly can be very complex, or even impossible (or intractable).

- This is where variational inference comes in. The neural network does not try to find the 
exact, true probability distribution of latent variables because this task is too difficult. 
Instead, it tries to find the variational distribution (often a Gaussian approximation) that 
is closest to the true distribution.

## <center> Neural Network Types<center/>
These are the different types of neural networks.

Each type is designed to solve specific challenges and make the most of DL.
***

### Convolutional Neural Networks (CNNs)
- excel at processing grid-like data, such as images or spatial information.

- CNN are inspired by the human visual cortex and are particularly effective at recognizing patterns, 
features in images, and objects.

Examples of CNN applications:
- **Image Classification** CNNs can identify objects, scenes and faces in images.

- **Object Detection** CNNs partition an image into multiple segments or regions, associating each with 
a specific class.

- **Image Segmentation** CNNs locate and identify objects in an image.

### Recurrent Neural Networks (RNNs)
- RNNs process information that comes in a specific order. This includes text, speech, or data generated 
over time, like time series data.

- RNNs have a special memory component. This component allows them to remember and use previous inputs,
like the previous word in a sentence. RNNs can then generate and predict new outputs, such as the next 
word in a sentence. They do this by considering the context of the previous words.

Examples of RNN applications:
- **Gesture Recognition** RNNs recognize and interpret human gestures from sensor data or video feeds.

- **Language Modeling** RNNs predict the next word or character in a sequence based on the previous context.

- **Named Entity Recognition** NER networks identify and classify the words in a sentence to different 
named entities, for example, people, organizations, or locations, in text data.


### Long Short-Term Memory (LSTM) Networks:
- LSTMs are variants of RNNs that are designed to remember information over a long period of time. This helps 
them overcome a problem that regular RNNs can have, where they have trouble learning relationships between 
information that is far apart.

- They have built-in memory cells that can selectively remember and forget information, as needed.

LSTMs often perform better, especially when dealing with long-range dependencies in the data.
- **Language Translation**

- **Sentiment Analysis** LSTMs are better equipped to handle long sentences and capture long-range 
dependencies between words, which is crucial for accurate translation.

- **Speech Recognition** LSTMs analyze text data, such as product reviews and social media posts, to 
determine the underlying sentiment or emotion.

- **Text Generation** LSTMs generate human-like text, such as creative writing, news articles, and poetry.

- **Time Series Forecasting** LSTMs predict future values based on historical data, like stock prices 
or weather patterns.

### Generative Adversarial Networks (GANs)
- GANs are generative models that are designed to generate new data that resemble the training data distribution. 

- GANs involve two neural networks (generator & discriminato) competing against each other in a zero-sum game framework.

- **Generator** This network generates new synthetic data (for example, images, text, or audio) by taking random noise 
as input and transforming it into data that resembles the training data distribution.

- **Discriminator** This network takes real data from the training set and synthetic data generated by the generator 
as input. 

Its goal is to distinguish between the real and generated data.


### Autoencoders


### Variational Autoencoders


## Transformer


## Self-supervised Learning