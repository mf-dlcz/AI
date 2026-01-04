# Inference Parameters
Parameters are used to customize the FM’s response. Generally, you should only adjust one parameter at a time, 
and the results can vary depending on the FM.


## Randomness and Diversity
### <ins>Temperature<ins>
- Temperature controls randomness in word choice
- LLMs use probability to construct the words in a sequence
- For any given sequence, there is a probability distribution of options for the next word in the sequence. 
- When you set the temperature closer to 0, the model tends to select the higher-probability words.
- When you set the temperature further from 0, the model might select a lower-probability word.
- Lower values lead to more predictable responses.

### <ins>Top K<ins>
- Top K controls the number of most-likely candidates that the model considers for the next token.
- A lower value decreases the size of the pool and limits the options to more likely outputs.
- A higher value increases the size of the pool and allows the model to consider less likely outputs.

### <ins>Top P<ins>
- This parameter controls choosing from the smallest number of tokens, where the combined, or cumulative, 
probability of the tokens exceeds the Top P parameter.
- A higher value for Top P, such as 0.9, implies that the output will be chosen at random from a larger 
number of tokens, which increases diversity. 
- However, a higher value can cause the output to become incoherent. 
- Lower values decrease the number of tokens available for selection, which increases the predictability of 
the next token.