# Foundation Models
Generative AI is powered by models that are pre-trained on internet-scale data, and 
these models are called foundation models (FMs).

FMs are large, general-purpose models pre-trained on vast amounts of diverse data, 
capturing broad knowledge and capabilities.

    - You can adapt or fine-tune these models for specific tasks or domains with 
    relatively small amounts of task-specific data and computational resources.
    
    - These tasks include text generation, text summarization, information 
    extraction, image generation, chat based assistant interactions, and question answering. 

Visualization:      
unlabeled data   ---- PRE-TRAINED ---->  Foundation Model ---- ADAPT ------->     BROAD RANGE OF GENERAL TASKS

## Benefits & Limitations
Creating an FM from scratch costs millions of dollars right now, they provide long-term benefits.

It's faster and cheaper for you to use pre-trained FMs to develop new ML applications.

This approach eliminates the need to train unique ML models from the ground up.

FMs, even through pre-trained, can adapt their responses based on data inputs or prompts during inference. 

This means that you can develop comprehensive outputs through carefully curated prompts.

Tasks that FMs can perform include language processing, visual comprehension, code generation, 
human-centered engagement, and speech to text.

### Foundation Model Benefits
1. **Language Processing**  
    They have remarkable capabilities to answer natural language questions and write short scripts or articles
    in response to prompts. They can translate languages using (NLP) technologies.

2. **Visual Comprehension**  
    Excel in computer vision, especially in regard to identifying images and physical objects. This is useful
    in autonomous driving and robots. Can generate images from input text, as well as photo and video editing.

3. **Code Generation**  
    Can generate computer code in various programming languages based on natural language inputs. Can debug code.

4. **Human-Centered Engagement**  
    Gen AI models use human input to learn and improve predictions. Potential uses include clinical diagnoses,
    decision support systems and analytics.

5. **Speech to Text**  
    Since FMs understand language, they can be used for speech-to-text tasks, such as transcription and video
    captioning, in a variety of languages.

FMs can respond coherently to prompts on subjects they have not been explicitly trained on.

### Foundation Model Limitations

1. **High cost**
    Building a FM from scratch is expensive and requires enormous resources, training might take months.

2. **Lack of comprehension**
    FMs have difficulty comprehending the context of a prompt. They aren't socially or psychologically
    aware.

3. **Unreliable answers**
    Answers to questions on certain subject matter might be unreliable and sometimes inappropriate, toxic,
    or incorrect.

4. **Bias**
    Models can pick up hate speech and inappropriate undertones from training datasets. To avoid, developers
    must carefully filter training data and encode specific norms into their models.


## How FMs work
FMs generate output from one or more inputs (or prompts). They use complex neural networks like transformers.

Each type of network functions differently, but they work on similar principles.

FMs use learned patterns and relationships to predict the next item in a sequence.

> [!NOTE]  
> FMs use self-supervised learning to create a language model during training.  
> This means no one has trained the model with labeled datasets.   
> This feature separates FMs from ML architectures, which use supervised and unsupervised learning.


## FM Lifecycle
- FM lifecycle is an iterative process. This means that lessons learned and insights gained from each stage
can inform and improve subsequent iterations.

1. **Data Selection**  
    Unlabeled data can be used at scale for pre-training because it is much easier to obtain compared to 
    labeled data. FM require training on massive datasets from diverse sources.

2. **Pre-Training**  
    FMs are typically pre-trained through self-supervised learning (labeled examples are not required).
    FMs algorithm can learn the meaning, context and relationship of the words in the datasets. After the
    initial pre-training, the model can be further trained on additional data to do specific tasks. This
    is known as _continuous pre-training_.

    _The goal is to expand the model's knowledge base and improve its ability to understand and generalize
    across different domains or tasks_.

3. **Optimization**
    The output of pre-trained language models can be optimized through techniques like prompt engineering,
    Retrieval Augmented Generation (RAG), and fine-tuning.

4. **Evaluation*
    Whether FM was fine-tuned or pre-trained, it's important to evaluate performance using metrics and 
    benchmarks.

5. **Deployment**
    When a FM meets performance criteria, it can be deployed to production environment. Deployment can involve
    integrating the model into applications, APIs, or other software systems.

6. **Feedback and Continuous Improvement**
    After deployment, the model's performance is continuously monitored, and feedback is collected from 
    users, domain experts, or other stakeholders. This feedback, along with model monitoring data, is 
    used to identify areas for improvement, detect potential biases or drift, and inform future iterations 
    of the model. The feedback loop permits continuous enhancement of the foundation model through 
    fine-tuning, continuous pre-training, or re-training, as needed.


## Types of FMs
Most common FMs are _text-to-text models_ and _text-to-image models_.


### Text-to-Text Models
Text-to-text models are large language models (LLMs) that are pre-trained to process vast quantities of textual 
data and human language. 

These large FMs can summarize text, extract information, respond to questions, create content (such as blogs or 
product descriptions), and more.


#### <ins>Natural Language Processing<ins>
Natural language processing (NLP) is an ML technology that gives machines the ability to interpret and 
manipulate human language.

NLP does this by analyzing the data, intent, or sentiment in the message and responding to human communication.

- Typically, NLP implementation begins by gathering and preparing unstructured text or speech data from 
different sources and processing the data.

- It uses techniques such as tokenization, stemming, lemmatization, stop word removal, part-of-speech 
tagging, named entity recognition, speech recognition, sentiment analysis, and so on.

NOTE: Modern LLMs don't require using these intermediate steps.


#### <ins>Recurrent Neural Network<ins>
Recurrent neural networks (RNNs) use a memory mechanism to store and apply data from previous inputs.

This mechanism makes RNNs effective for sequential data and tasks, such as NLP, speech recognition, or 
machine translation.

RNNs also have limitations. They are slow and complex to train, and they can’t be used for 
training parallelization.


#### <ins>Transformer<ins>
A transformer is a deep-learning architecture that has an encoder component that converts the input 
text into embeddings. 

It also has a decoder component that consumes the embeddings to emit some output text. 

Unlike RNNs, transformers are extremely parallelizable. 

This means that instead of processing text words one at a time during the learning cycle, transformers 
process input all at the same time.

It takes transformers significantly less time to train, but they require more computing power to speed 
training. The transformer architecture was the key to the development of LLMs. 

These days, most LLMs only contain a decoder component.


### Text-to-Image Models
Text-to-image models take natural language input and produce a high-quality image that matches the 
input text description.


## Multi-modal Models
- Multi-modal models can process and generate multiple modes of data simultaneously.

- For example, a multi-modal model could take in an image and some text as input, and 
then generate a new image and a caption describing it as output.


# Inference Parameters
- Inference, in machine learning, is the process of using a trained model to make predictions or generate 
outputs based on new, unseen input data.

- It is the phase where the model is deployed and used to solve real-world problems. 

- When interacting with FMs, you can often configure inference parameters to limit or influence the 
model response.

- Inference parameters fit into a range of categories, with the most common being _randomness, 
diversity, and length._


## Randomness and Diversity
- Randomness and diversity are the most common categories of inference parameters.

Randomness and diversity parameters influence the variation in generated responses by limiting the outputs to 
more likely outcomes or by changing the shape of the probability distribution of outputs.


### <ins>Temperature<ins>
- This parameter controls the randomness or creativity of a model's output. 
- A higher temperature makes the output more diverse and unpredictable, and a lower temperature makes it 
    more focused and predictable. 
- Temperature is set between 0 and 1.


### <ins>Top K<ins>
- Top K limits the number of words to the Top K most probable words, regardless of their percent probabilities.

- For example, if Top K is set to 50, the model will only consider the 50 most likely words for the next 
word in the sequence.


### <ins>Top P<ins>
- Top P is a setting that controls the diversity of the text.

- This is done by limiting the number of words that the model can choose from based on their cumulative 
probabilities.

- At each step, the model ranks the potential next tokens by their predicted probabilities. 

- Top P specifies a threshold probability value between 0 and 1.


## Fine-Tuning
- Fine-tuning an FM base model can improve performance.

- Fine-tuning is a supervised learning process that involves taking a pre-trained model and adding specific, 
smaller datasets.

- Adding these narrower datasets modifies the weights of the model to better align with the task.

- There are two ways to fine-tune a model: _**instruction fine-tuning and reinforcement learning from human feedback 
(RLHF)**._


### <ins>Instruction Fine-Tuning<ins>
- Instruction fine-tuning is a type of supervised machine learning.

- You make the FMs interact like a human in its interactions (inputs and generated outputs).

- You provide a small set of inputs (usually fewer than 1,000) as examples of how to handle a specific task, such 
as summarization.

- You then give instructions to the model and compare its generated output with the correct output (this is called 
ground truth labels in machine learning).

- After going through this process many times, you give the model feedback about its performance. 

- The model then updates its weights to improve its predictions in the future.

- Consider that if you fine-tune the model to do only one thing in your instructions, you make the model better 
at doing that one task. But it might lose its ability to perform other tasks as well as before. 

- This is called catastrophic forgetting. 


### <ins>Reinforcement Learning from Human Feedback<ins>
- Reinforcement learning from human feedback (RLHF) provides human feedback data, resulting in a model that 
is better aligned with human preferences. 

- RLHF is most applied after one form of fine-tuning, such as instruction fine-tuning. 