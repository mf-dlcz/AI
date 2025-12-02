# Large Language Models
- LLMs are a subset of FMs.

- LLMs are trained on trillions of words across many natural language tasks.

- The main goal of a language model is to predict the chance of a sequence of words 
happening together sensibly.


## Large models compared to large language models
Language models present two major challenges

1. They process input sequences one element at a time in a sequential manner.
It limits parallelization.

2. They have difficulty with very long-range dependencies in tasks like language modeling or
machine translation for long sequences.

- The breakthrough of LLMs is that they use a transformer architecture to solve those problems
through _positional encoding_ and _self-attention_.

- The word _large_ in LLM comes from the fact that LLMs can consider billions of parameters and 
have many possible uses.


# How LLMs Work
- LLMs can be based on a variety of architectures, but the most common architecture today is the
transformer architecture.

- Transformer-based LLMs are powerful models that can understand and generate human-like text.


## Tokens
Tokens are the basic units of text that a model processes.

Tokens can be words, phrases, or individual characters, like a period.

This sentence might be broken into the following 11 tokens: A, puppy, is, to, dog, as, a, kitten, 
is, to, cat.


## Embedding Vectors
Embeddings are numerical representations of tokens.

Each token is assigned a vector (a list of numbers) that captures its meaning and relationships with 
other tokens.

These vectors are learned during the training process and allow the model to understand the context 
and nuances of language.


> [!NOTE]  
> LLMs use these tokens, positional embeddings, and self-attention to understand and generate text.


## Layers in Transformer Models
 These layers might include embedding, positional encoding, attention, feed-forward, normalization, 
 soft-max, and linear layers. 


### <ins>Embedding Layer<ins>
The embedding layer converts input text to vector representations called input embeddings. This 
happens through a tokenizer first and then embedding the tokens.


### <ins>Positional Encoding Layer<ins>
The positional encoding layer encodes the position of each word in a sequence to allow the model 
to understand word order and position. Positional encoding is crucial for capturing context, as 
the meaning of a word can change depending on its position in a sequence.


### <ins>Attention Layer<ins>
The attention layer replaces the recurrence mechanism found in RNNs and LSTMs, eliminating the 
need for sequential processing of inputs.

The attention layer adeptly embeds contextual information into each incoming word. 

This is accomplished by assessing the importance and relevance of every word concerning all other 
words in the sequence. 

By doing so, the model comprehends the interdependencies and relationships between words in the 
input, enabling a deeper understanding of the overall context.


### <ins>Feed-forward Layer<ins>
The feed-forward layer in encoder and decoder consists of several connected networks that use the 
output of self-attention layer. Essentially, this layer continues to contextualize the language 
and helps the model better understand the input text's intent.