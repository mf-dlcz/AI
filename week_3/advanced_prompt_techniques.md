# Advanced Prompt Techniques
Basic prompt techniques don't always provide the results that you need for your specific business tasks.


## Self-Consistency
Self-consistency is a prompting technique that is similar to chain-of-thought prompting. However, instead 
of taking the obvious step-by-step, or greedy path, self-consistency prompts the model to sample a variety 
of reasoning paths. Then, the model aggregates the final answer based on multiple data points from the 
various paths.

### Self-Consistency Prompt Example
_Prompt_:  
Q. Terry had 12 apples. He gave half to Jane. John gave Terry three more apples. How many apples does 
Terry have?
A. Terry originally had 12 apples. He gave half to Jane, which means he gave 6 away. So now, Terry has 
12 − 6 = 6 apples. John gave Terry three more apples, which means 3 + 6, so Terry now has 9 apples.

Q. When I was 10, my sister was half my age. Now I’m 40 years old. How old is my sister?
A.

_Output:_  
When I was 10, my sister was 10/2 = 5 years old.

Now, I’m 40, so my sister is 40 − 5 = 35 years old.


## Tree of Thought (ToT)
Tree of thoughts (ToT) is another technique that builds on the CoT prompting technique. 

CoT prompting samples thoughts sequentially, but ToT prompting follows a tree-branching technique. 

With the ToT technique, the LLM can learn in a nuanced way, considering multiple paths instead of one 
sequential path.

_ToT prompting is an especially effective method for tasks that involve important initial decisions, 
strategies for the future, and exploration of multiple solutions._


## Retrieval Augmented Generation (RAG)
Retrieval Augmented Generation (RAG) is a prompting technique that supplies domain-relevant data as 
context to produce responses based on that data and the prompt.

This technique is similar to fine-tuning. However, rather than having to fine-tune an FM with a small set 
of labeled examples, RAG retrieves a small set of relevant documents from a large corpus and uses that to 
provide context to answer the question. RAG will _not_ change the weights of the foundation model, whereas 
fine-tuning will change model weights.

RAG approach doesn't incur the cost of fine-tuning a model.

RAG also addresses the challenge of frequent data changes because it retrieves updated and relevant 
information instead of relying on potentially outdated sets of data.


## Automatic Reasoning and Tool-use (ART)
ART is a prompting technique that builds on the chain-of-thought process.

ART is used specifically for multi-step reasoning tasks.

This technique essentially deconstructs complex tasks by having the model select demonstrations of 
multiple, or few-shot, examples from the task library. 

At the same time that the model is using this few-shot breakdown, it uses predefined external tools such 
as search query and code generation to carry out the task.


## ReAct Prompting
With ReAct prompting a LLM can combine reasoning and action.

LLMs are often used for reasoning or for acting, but they are not always effectively used for both at 
the same time.