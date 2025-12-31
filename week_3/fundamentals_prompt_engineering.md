# Prompt Engineering Overview
- Prompt engineering is different from fine-tuning.
- In fine-tuning, the weights or parameters are adjusted using training data with the goal of 
optimizing a cost function. 
Fine-tuning can be an expensive process, both in terms of computation time and actual cost. 

- Prompt engineering, however, attempts to guide the trained FM, an LLM, or a text-to-image 
model, to give more relevant and accurate answers.

## Elements of a prompt
A prompt's form depends on the task that you are giving to a model.

- **Instructions:** It provides a task description or instruction for how the model should perform.

- **Context:** This is external information to guide the model.

- **Input Data:** This is the input for which you want a response.

- **Output Indicator:** This is the output type or format.

## Best Practices for Designing Effective Prompts
- **Be clear and concise:**  Craft prompts with natural, flowing language and coherent sentence 
structure.

- **Include context if needed:** Provide any additional context that would help the model respond 
accurately.

- **Use directives for the appropriate response type:** Specify the response type directly (summary, 
question, or poem). You can also limit responses by length, format, included information, excluded 
information, and more.

- **Consider the output in the prompt:** Mention the requested output at the end of the prompt to 
keep the model focused on appropriate content.

- **Start prompts with an interrogation:** Phrase your input as a question, beginning with words 
such as who, what, where, when, why, and how.

- **Provide an example response:** Use the expected output format as an example response in the 
prompt. Clarify that the model is to follow the format of the examples in the prompt.

- **Break up complex tasks:** 
    1. Divide the task into several subtasks. If you cannot get reliable results, try splitting 
    the task into multiple prompts.

    2. Ask the model if it understood your instruction. Provide clarification based on the 
    model's response.

    3. If you don’t know how to break the task into subtasks, ask the model to think step by step. 

- **Experiment and be creative:** Try different prompts to optimize the model's responses.