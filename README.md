# aidp
The AI Democracy Projects are a collaboration between [Proof News]([url](https://www.proofnews.org/)) and the [Science, Technology, and Social Values Lab]([url](http://www.ias.edu/stsv-lab)) at the Institute for Advanced Study.

This repository contains data from our pilot for domain-specific safety testing conducted in January 2024. Auditing Evaluating five leading AI models’ responses to election-related prompts for bias, accuracy, completeness, and harmfulness, this testing engaged state and local election officials, AI experts from research and civil society organizations, academics, and journalists. The models tested were Anthropic’s Claude, Google’s Gemini, OpenAI’s GPT-4, Meta’s Llama2, and Mistral’s Mixtral. For GPT-4, Gemini, and Claude, we used the original provider APIs directly. For the open models — Llama2 and Mixtral — we used Deep Infra, a service that hosts and runs a variety of machine learning models.

We divided the roughly 40 experts into teams. Each team of 2-6 people voted on whether to rate a models' answer to a given prompt inaccurate, hamful, incomplete, and/or biased. 

See our report here.

See our methodology here.

*Data Dictionary*
 
group_id, unique id given to every team of raters
user_prompt, text of prompt run through each model
panel_size, number of members on rating team associated with group_id
model, LLM name
answer, response generated by LLM to user_prompt
inaccurate, number of members of testing team (group_id) who voted to identify user_prompt as inaccurate
harmful, number of members of testing team (group_id) who voted to identify user_prompt as harmful
incomplete, number of members of testing team (group_id) who voted to identify user_prompt as incomplete
biased, number of members of testing team (group_id) who voted to identify user_prompt as biased




