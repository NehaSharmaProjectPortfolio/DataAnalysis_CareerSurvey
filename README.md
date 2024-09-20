# Data Analysis of data on online career survey for transition to Data Careers.
---
## Table of Contents
- [Project Objective](#project-objective)
- [Tools](#tools)
- [AI Model Details](#ai-model-details)
- [DataSets](#datasets)
- [Project Steps](#project-steps)
- [Results](#results)
---
### Project Objective: To study dialogue summarization task using generative AI Pre-Trained LLM Model (FLAN-T5) and impacts of prompt engineering to achieve desired outcomes.
* We will explore the impact of input text on the output of the model
* Then we will further perform prompt engineering to attempt to achieve the desired summarization against the human labelled benchmark. 
* Next we perform zero shot, one shot, and few shot inferences and observe how it can enhance the generative output of Large Language Models like FLAN-T5 Model
---
### Tools
- `Amazon SageMaker` :  We used Amazon SageMaker and its studio to load and deploy Gen AI LLM Model for our use case with fully managed infrastructure, tools, and workflows. The Configuration details are (ml.m5.2xlarge)
- `Python`:
           We have written python code for loading the FLAN-T5 model and the test datasets from Hugging Face.
           We installed Pytorch and Hugging Face transformers and datasets modules and respective functions.
---
### AI Model Details
- Pre-trained Large Language Model(LLM) FLANT-5 from Hugging Face
- List of avialable models and documentation from Hugging Face can be referred [here](https://huggingface.co/docs/transformers/index)
___
### DataSets 
- The career survey dataset [DialogSum](https://huggingface.co/datasets/knkarthick/dialogsum) 
---
### Project Steps
* Step 1: We installed the required packages PyTorch and Hugging Face transformers and datasets.
* Step 2: Load the datasets, Large Language Model (LLM), tokenizer, and configurator.
* Step 3: Load the FLAN-T5 model, creating an instance of the AutoModelForSeq2SeqLM class with the .from_pretrained() method.
* Step 4: To perform encoding and decoding, you need to work with text in a tokenized form. Tokenization is the process of splitting texts into smaller units that can be processed by the LLM models.
* Step 5: Testing the tokenizer encoding and decoding a simple sentence.
* Step 6: Tokenizer is working fine its validated. Now it's time to explore how well the base LLM summarizes a dialogue without any prompt engineering. Prompt engineering is an act of a human changing the prompt (input) to improve the response for a given task.
* Step 7: Test the response of the model *without prompt engineering*<br/>
**Observation:** We see that the guesses of the model make some sense, but it doesn't seem to be sure what task it is supposed to accomplish. Seems it just makes up the next sentence in the dialogue.
* Step 8: Test the response of the model with *zero shot and few shot prompts*.<br/>
**Observation:** This is much better! But the model still does not pick up on the nuance of the conversations though.
---
### Results
* In this case, few shot did not provide much of an improvement over one shot inference.
* And, anything above 5 or 6 shot will typically not help much, either.





Dialogue:

* [Hugging Face Models Documentation](https://huggingface.co/docs/transformers/index)

# DataAnalysis with PowerBI
Data Analysis Projects

## PowerBI Dashboard
![PowerBI Dashboard for Career Survey](https://github.com/NehaSharmaProjectPortfolio/DataAnalysis_CareerSurvey/blob/main/DataCareerSurvey.png)
