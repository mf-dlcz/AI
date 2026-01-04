# Overview of the Amazon Bedrock API
The following tools can be used to set up an environment to make Amazon Bedrock requests through the
Amazon Bedrock API.

1. AWC CLI
2. AWS SDKs


## How to invoke a model using the Amazon Bedrock API
**Create an endpoint connection:**  
The Amazon Bedrock endpoints allow you to interact with the Amazon Bedrock service and its FMs.

There are several kinds of endpoints, and they provide their own unique API operations for a variety of tasks,
such as these:
- Creating, managing and evaluating models
- Creating provisioned models
- Getting foundation models
- Getting guardrails
- Getting model customization jobs

#
**Specify Parameters:**  
You can set parameters for both Amazon Bedrock and for the FM you are using.

#
**Pass a Prompt and any Model-Specific Parameters:**  
Next, pass your prompt to the FM and combine it with FM-specific parameters. This creates the prompt body.

#
**Invoke your FM and Format the Output:**  
Once you have entered your prompt, you need to invoke your FM and specify your preferred output format.