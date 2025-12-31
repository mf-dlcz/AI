# Basic Prompt Techniques
When crafting and manipulating prompts, there are certain techniques that you can use to achieve the 
response you want from AI models.

## Zero-Shot Prompting
Zero-shot prompting is a prompting technique where a user presents a task to an LLM without giving the 
model further examples.

The user expects the model to perform the task without a prior understanding, or shot, of the task.

### Tips for Using a Zero-Shot Prompting Technique:
- The larger the LLM, the more likely the zero-shot prompt will yield effective results.

- Instruction tuning can improve zero-shot learning. You can adopt reinforcement learning from human 
feedback (RLHF) to scale instruction tuning, to align modern LLMs to better fit human preferences.


## Few-Shot Prompting
Few-shot prompting is a prompting technique where you give the model contextual information about the 
requested tasks.

In this technique, you provide examples of both the task and the output you want.

Providing this context, or a few shots, in the prompt conditions the model to follow the task guidance 
closely.

### Tips for Using a Few-Shot Prompting Technique:
- The labels in a few-shot prompt do not have to be correct to improve model performance. 
Usually, applying random labels outperforms using no labels at all. 
However, the label space and distribution of the input text specified by the demonstrations are important. 
The use of the term label in this context refers to the output of the prompt examples.

- If you have access to a large set of examples, use techniques to obey the token limits of your model and 
dynamically populate prompt templates. 
You can use an example selector that is based on semantic similarity to help.


## Chain-of-thought Prompting
Chain-of-thought (CoT) prompting breaks down complex reasoning tasks through intermediary reasoning steps.

You can use both zero-shot and few-shot prompting techniques with CoT prompts.

Chain-of-thought prompts are specific to a problem type. You can use the phrase "Think step by step" to 
invoke CoT reasoning from your ml model.

### Tips for Using Chain-of-thought Prompting Technique:
- Use CoT prompting when the task involves several steps or requires a series of reasoning.