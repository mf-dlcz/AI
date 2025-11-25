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
unlabeled data   ---- PRE-TRAINED ---->  Foundational Model ---- ADAPT ------->     BROAD RANGE OF GENERAL TASKS

## Benefits & Limitations
Creating an FM from scratch costs millions of dollars right now, they provide long-term benefits.

It's faster and cheaper for you to use pre-trained FMs to develop new ML applications.

This approach eliminates the need to train unique ML models from the ground up.

FMs, even through pre-trained, can adapt their responses based on data inputs or prompts during inference. 

This means that you can develop comprehensive outputs through carefully curated prompts.

Tasks that FMs can perform include language processing, visual comprehension, code generation, 
human-centered engagement, and speech to text.

### Foundational Model Benefits
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

### Foundational Model Limitations

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

> NOTE!  
> FMs use self-supervised learning to create a language model during training. 
> This means no one has trained the model with labeled datasets. 
> This feature separates FMs from ML architectures, which use supervised and unsupervised learning.


## FM Lifecycle
- FM lifecycle is an iterative process. This means that lessons learned and insights gained from each stage
can inform and improve subsequent iterations.

1. **Data Selection**  
    Unlabeled data can be used at scale for pre-training because it is much easier to obtain compared to 
    labeled data. 