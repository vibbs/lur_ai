2023-05-31
## What is a LLM?

A large language model is a machine learnt model on vareity of data which exists across the internet. 



## What happens when you send a prompt to LLM?

Internally based on the trained data set the model is actually not giving you a response to your prompt, it is actually building the output response token by token(think on the lines of word by word). And when generating a new token it is probabilistically choosing the next token based on the trained data set. This might seem like a cognitive process but it is not. It is just a mathematical process.


## What are some different types of LLMs?

### Pre-trained LLMs

Examples: GPT-2, GPT-3, BERT, etc.

Let's say you want to ask the internet to give you information about best food in a certain part of the world, you will get a lot of information. Some of the those information would be in different languages. So, you will have to translate them to your language.

In the LLMs let's assume that the model is also trained on the this data set which has understood the contextual meaning of the data set. So, when you ask the model, the model will try to give you the best answer based on the data set it is trained on but linking the likelyhood of the answer to the data set.

There is a downfall of this as well, let's say the model is trained on 10 food blog articles out of which 5 of them are not credible sources. So, you will start to see responses which are inaccurate.


### Fine-tuned LLMs or Instruction tuned LLMs

Examples: ChatGPT, Alpaca, Codex, etc.

Building on top of Pre-trained LLMs, where certain instructions are provided to train the model to remove the bias and to give more accurate results.

So expanding on the above example if we are able to deterministically provide proper data set for the model to distinguish between credible and non-credible sources, then the model will be able to give more accurate results.

Another example to think about Fine-tuned LLMs let's say we ask for what is best place to each a certain best food for a given location a general model will give probably a list of places to eat but a fine-tuned model will give you a list of places to eat considering the rating and a review - if we have fine tuned or instructed the model to do so.

Another Instruction Tuned LLms example is let's say you trained a langauge model with all open source code bases and you want to use it to generate code for a specific language, then you will have to fine tune the model to generate code for a specific language. This is what we call as Instruction Tuned LLMs. And **GitHub Copilot** is an example of this.

### Agent Simulation LLMs

Examples: User Defined or Custom LLM Applications. 

Continuing on our example of food, let's say we want to build a food recommendation app. We will have to build a model which will be able to understand the context of the user and will be able to give the best results. This is what we call as Agent Simulation LLMs.

Like an example input from the user might be: "Give me a best food to eat". And the recommendation app takes in the input and context like location from the user metadata or some form of filter and gives the best results. Designing the expected output which can be then disaplyed to user with proper review rating and other information is what constitutes the Agent Simulation LLMs.

So caracteristics of Agent Simulation LLMs for the above examples are:
- User input
- Context - User metadata
- Trained data set - Food reviews, ratings, etc.
- Output - Structured data set of food recommendations





