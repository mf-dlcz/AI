# Basics of FMs
- Gen AI is powered by ML models.

- The large models are called FMs.

- FMs are typically pre-trained through self-supervised learning.


## Foundation Model Functionality
- FMs use deep neural networks to emulate human brain functionality to handle complex tasks. 

- You can adapt them for a broad range of general tasks, such as 
    - text generation
    - text summarization
    - information extraction
    - image generation
    - chat-based assistant
    - question answering 
    
- FMs can also serve as the starting point for developing more specialized models.

_Unlabled data is used to pre-train a FM which adapts to generate a broad range of general tasks._


## Self-Supervised Learning
- FMs are typically pre-trained through self-supervised learning. With self-supervised learning, labeled 
examples are not required. Self-supervised learning makes use of the structure within the data to 
autogenerate labels.

### Training, Fine-Tuning, and Prompt Tuning
Foundation models go through various stages of training to achieve the best results.

### <ins>Pre-Training<ins>
- During the training stage, FMs use self-supervised learning or reinforcement learning from human feedback 
(RLHF) to capture data from vast datasets. 

- The FM's algorithm can learn the meaning, context, and relationship of the words in the datasets.

- In addition, RLHF technique can be used during pre-training to better align the model with human 
preferences. In this approach, humans provide feedback on the model outcomes, and that information is used 
by the model to change its behavior.

### <ins>Fine-Tuning<ins>
- Though FMs are pretrained through self-supervised learning and have inherent capability of understanding 
information, fine-tuning the FM base model can improve performance. 

- Fine-tuning is a supervised learning process that involves taking a pretrained model and adding specific, 
smaller datasets. Adding these narrower datasets modifies the weights of the data to better align with the 
task.

There are two ways to fine-tune a model:
1. **Instruction fine-tuning** uses examples of how the model should respond to a specific instruction. 
Prompt tuning is a type of instruction fine-tuning.

2. **RLHF** provides human feedback data, resulting in a model that is better aligned with human preferences.

### <ins>Prompt Engineering<ins>
- Prompts act as instructions for foundation models. 

- They are similar to fine-tuning, but you don’t need to provide labeled sample data as you would to 
fine-tune a model. 

- You use various prompt techniques to achieve better performance. 

- Prompt engineering is a more efficient way to tune LLM responses, as opposed to fine-tuning, which 
requires labeled data and training infrastructure.


## Types of FMs
- FMs can be categorized into multiple categories. Two of the most frequently used models are 
text-to-text models and text-to-image models.

### <ins>Text-to-Text Models<ins>
- Text-to-text models are LLMs that are pre-trained to process vast quantities of textual data and 
human language.

### <ins>Text-to-Image Models<ins>
- Diffusion is a deep learning architecture system that learns through a two-step process. The first step 
is called forward diffusion. Using forward diffusion, the system gradually introduces a small amount of 
noise to an input image until only the noise is leftover. There is a U-Net model, which tracks and predicts 
the noise level. In the subsequent reverse diffusion step, the noisy image is gradually introduced to 
denoising until a new image is generated. During the training process, the model gets the feed of text, 
which is added to the image vector.

### <ins>Natural Language Processing (NLP)<ins>
- NLP is a machine learning technology that gives machines the ability to interpret and manipulate 
human language.

- NLP does this by analyzing the data, intent, or sentiment in the message and responding to human 
communication. 

### <ins>Recurrent Neural Network (RNN)<ins>
- RNNs use a memory mechanism to store and apply data from previous inputs.

- Effective for sequential data and tasks, such as natural language processing, speech recognition, or 
machine translation.

- They are slow and complex to train, and they can’t be used for training parallelization.

### <ins>Transformer<ins>
- A transformer is a deep-learning architecture that has an encoder component that converts the input text 
into embeddings. It also has a decoder component that consumes the embeddings to emit some output text.

- transformers are extremely parallelizable, which means that instead of processing text words one at a 
time during the learning cycle, transformers process input all at the same time.

- It takes transformers significantly less time to train, but they require more computing power to speed 
training. The transformer architecture was the key to the development of LLMs. These days, most LLMs 
only contain a decoder component.


## LLMs
- LLMs are a subset of foundation models. 

- LLMs are trained on trillions of words across many natural language tasks.

### <ins>Understanding LLM Functionality<ins>
- Most LLMs are based on a transformer model. They receive the input, encode the data, and then decode 
the data to produce an output prediction.

### <ins>Neural Network Layers<ins>
- Transformer models are effective for natural language processing because they use neural networks to 
understand the nuances of human language. 

- There are multiple layers of neural networks in a single LLM that work together to process input 
and generate output.

### <ins>Embedding Layer<ins>
- The embedding layer converts input text to vector representations called embeddings.

- This layer can capture complex relationships between the embeddings, so the model can understand the 
context of the input text.

### <ins>Feed-Forward Layer<ins>
- The feedforward layer consists of several connected layers that transform the embeddings into more 
weighted versions of themselves.

- Essentially, this layer continues to contextualize the language and helps the model better understand 
the input text's intent.

### <ins>Attention Mechanism<ins>
- With the attention mechanism, the model can focus on the most relevant parts of the input text.

- This mechanism, a central part of the transformer model, helps the model achieve the most accurate 
output results.