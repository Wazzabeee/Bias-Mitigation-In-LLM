# Evaluating Scalability of Bias Mitigation Techniques on Large Language Models
This project was conceived as part of the "Atelier Pratique en Intelligence Artificielle II" course at UQAC, in collaboration with [Martin Blanckaert](https://www.linkedin.com/in/martinblanckaert/), [Valentin Porchet](https://www.linkedin.com/in/valentin-porchet/), [Thomas Sirvent](https://www.linkedin.com/in/tsirvent/) and under the supervision of [Darine Ameyed](https://scholar.google.com/citations?user=uoP1tAMAAAAJ) and [Riadh Ben Chaabene](https://ca.linkedin.com/in/riadh-ben-chaabene).

## Objective

The objective was to produce a proof of concept in 2 months on a research topic of our choice. We focused on bias mitigation in large language models. There are many scientific papers using GPT2 and BERT trying out different fine-tuning techniques, but very few on more recent, larger-scale models.

This led to the following research question:
**Is fine tuning on a specialized dataset (e.g. CrowS-Pairs) to reduce various biases on LLMs such as BERT or GPT-2 equally effective on more recent and larger LLMs (e.g. Bloomz or FLAN-T5)?**

## Repository

In this repo you'll find our article in X.pdf as well as our various notebooks for reproducing our results.

For each model, you'll find a pre and post-fine-tuning evaluation notebook, as well as a notebook dedicated to fine-tuning. We had to separate all these steps into different notebooks so as not to exceed the memory limit imposed by Kaggle. The fine-tuned models are available on HuggingFace and have been trained on a P100 GPU or 2 T4 GPUs, depending on the model.

## Our Work
To measure model bias, we propose two sets of metrics. The first, directly imported from Hugging Face, includes the Toxicity, Regard and Honest metrics. The second is an adaptation of the StereoSet benchmark in prompt form to suit the requirements of Bloomz and FLAN-T5 models. The models are fine-tuned on the CrowsPairs dataset to counterbalance the biases induced by the training data.

## Results
*To be completed*
