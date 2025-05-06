# LLM-Self-Correction-and-IRT

This project provides a diagnostic framework for evaluating LLM self-correction capabilities using error typology and Item Response Theory

---

## Table of Contents

- [About The Project](#about-the-project)
- [installation](#getting-started)

---

## About The Project

This is a course project for the course NLP804 Deep Learning for Natural Language Generation. In this project, I look into 4 prompts for self correction and observe LLM behaviours of the models GPT-4o, DeepSeek-R1, Phi4 and Gemma3, in the presence or absence of information about an error made in an LLMs solution. Additionally, I apply Item Response Theory to empirically compare proficienct levels to an average 12th grader that took the NAEP exams. 

### **1. `IRT/`**
Contains implementations for the experiments and calculations done for the IRT aspect of the project

- **`naep_data`**: 
  - 'parameters/' has all questions ids and their parameters from the NAEP website. 
  - 'questions/' has 4 NAEP csv files that matches questions from the json NAEP file to its IRT parameters. Some may be empty

- **`responses_mcq`**: 
  - contains all LLM responses 

  
### **2. `self_correct/`**
Contains implementations the self correction experiments. 

- **`data/`**: 
  - Folder for all preprocessed data samples and generated responses from the LLMs 

- **`evaluation/`**: 
  - Folder for all code to create graphs for the self correction attempts. 

- **`inferencing/`**: 
  - Scripts for prepping data and inferring responses from the 4 LLMs. 
---

## Installation

To install this repo:
```
conda create -n NLG_project python=3.11 
conda activate NLG_project
pip install -r requirements.txt
```