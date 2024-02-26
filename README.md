# aidp
The AI Democracy Projects are a collaboration between [Proof News](https://www.proofnews.org/) and the [Science, Technology, and Social Values Lab](http://www.ias.edu/stsv-lab) at the Institute for Advanced Study.

This repository contains data from our pilot for domain-specific safety testing conducted in January 2024. Evaluating five leading AI models’ responses to election-related prompts for bias, accuracy, completeness, and harmfulness, this testing engaged state and local election officials, AI experts from research and civil society organizations, academics, and journalists. The models tested were Anthropic’s Claude, Google’s Gemini, OpenAI’s GPT-4, Meta’s Llama 2, and Mistral’s Mixtral. For GPT-4-0613, and Claude-2 with Anthropic version 2023-06-01, we used the original provider APIs directly. For the open models — Llama-2-70b-chat-hf and Mixtral-8x7B-Instruct-v0.1 — we used Deep Infra, a service that hosts and runs a variety of machine learning models. For Gemini Pro Preview (last update Dec. 13, 2023) we used a hosting service called OpenRouter. 

We divided the roughly 40 experts into teams. Each team of two to six people voted on whether to rate a model's answer to a given prompt as inaccurate, hamful, incomplete, and/or biased. 

See our report [here](https://www.proofnews.org/seeking-election-information-dont-trust-ai).

See our methodology [here](https://www.proofnews.org/how-we-tested-leading-ai-models-performance-on-election-queries).

*Data Dictionary*

|Column | Description |
|-------| ----------- |
|group_id |unique id given to every team of raters |
|user_prompt | text of prompt run through each model |
|panel_size | number of members voting on rating team associated with group_id |
|model | LLM name | response generated by LLM to user_prompt|
|answer | model's response to user_prompt |
|inaccurate | number of members of testing team (group_id) who voted to identify user_prompt as inaccurate|
|harmful |number of members of testing team (group_id) who voted to identify user_prompt as harmful|
|incomplete | number of members of testing team (group_id) who voted to identify user_prompt as incomplete|
|biased | number of members of testing team (group_id) who voted to identify user_prompt as biased|




