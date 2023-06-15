<div align= "center">
    <h1> 🛠️ToolQA</h1>
</div>

🛠️ The official repository for code and data of ToolQA dataset. ToolQA is a open-source dataset specifically designed for evaluations on tool-augmented large language models (LLMs). We provide the dataset, the corresponding data generation code, and the implementations of baselines on our dataset.

## Features

- Our questions are selected and guaranteed that **LLMs have little chance to memorize and answer correctly within their internal knowledge**;
- The majority of the questions in ToolQA **require compositional use of multiple tools**. According to the length of toolchains, we offer two different difficult levels of dataset: **Easy** and **Hard**.
- We apply **a thorough diagnosis and analysis of in-context tool-augmented LLMs** in our paper.
- ToolQA is **a human-AI collaborated dataset** that can automatically be applied on the other new data and questions.

<p align="center">
  <img 
    width="800"
    src="./figure/overview.png"
  >
</p>

## Data Download
We offer the download link for all the data involved in ToolQA. We offer two categories of data for download and use. The first category is **external corpus**. This sort of data have already been pre-processed by us and they are used for external tools to interact, (e.g., retrieve, database operations, etc.). The second category of data is the **raw data**, which cannot be used as external knowledge of ToolQA to interact. We offer this part of data just for users if they want to generate more questions and answers for model tuning or thorough evaluation.

### External Corpus Download
The external corpus can be downloaded through [this link](https://drive.google.com/file/d/1zRbHzPW2x4dDcfmphBWlan8cxUCRNmqk/view?usp=drive_link). After download and unzip, users need to place it under the directory  ``/<YOUR_OWN_PATH>/ToolQA/data/external_corpus/``.

### Raw Data Download
All the data sources and download guidance are listed below:
- **Flight**: You can download the raw flight data from the [Download Link](https://www.kaggle.com/datasets/robikscube/flight-delay-dataset-20182022?select=Combined_Flights_2022.csv). Please place the ``Combined_Flights_2022.csv`` file under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/flights/``.
- **Coffee**: You can download the raw coffee data from the [Download Link](https://www.kaggle.com/datasets/psycon/daily-coffee-price). Please place the ``coffee.csv`` file under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/coffee/``.
- **Yelp**: You can download the raw yelp data from the [Download Link](https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset?select=yelp_academic_dataset_business.json). Please place the ``yelp_academic_dataset_business.json`` file under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/yelp/``.
- **Airbnb**: You can download the raw airbnb data from the [Download Link](https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata). Please place the ``Airbnb_Open_data.csv`` file under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/airbnb/``.
- **DBLP**: You can download the raw dblp data from the [Download Link](https://www.aminer.org/citation). Please place the ``DBLP-Citation-network V14.zip`` file under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/dblp/``.
- **GSM8K**: You can download the raw dblp data from the [Download Link](https://github.com/openai/grade-school-math). Please run ChatGPT vanilla on the raw questions and place the result file ``gsm.chat.jsonl`` under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/gsm8k/``.
- **SciREX**: You can download the raw dblp data from the [Download Link](https://github.com/allenai/SciREX). Please place the dataset files ``train.jsonl``, ``val.jsonl``, and ``test.jsonl`` under the directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/scirex/``.
- **Agenda**: You can download the raw data from our prepared [Download Link](https://drive.google.com/file/d/1A-DP_EFGVglaXf6-RUzN2Oq4rB58jExG/view?usp=drive_link). Please place the file ``agenda_events.jsonl`` underthe directory ``/<YOUR_OWN_PATH>/ToolQA/data/raw_data/agenda/``.

### Generate New Questions
You can also use the ToolQA to generate new questions under our templates for tuning and new sets of evalations. We offer the data generation code in `/dataset_generation/` directory. The only thing to do is to modify the paths in the notebooks.


## Current Progress
The data and code are in the final stage of clean and will be public gradually in a very short period. We offer the detailed progress of the final examination in the TODO list part.

### To Do List -- Easy Questions
- [x] ~~Flight-easy questions and code;~~
- [x] ~~Coffee-easy questions and code;~~
- [x] ~~Yelp-easy questions and code;~~
- [x] ~~Airbnb-easy questions and code~~;
- [x] ~~SciREX-easy questions and code;~~
- [x] ~~Agenda-easy questions and code;~~
- [x] ~~GSM8K-easy questions and code;~~
- [x] ~~DBLP-easy questions and code;~~

### To Do List -- Hard Questions
- [x] ~~Flight-hard questions and code;~~
- [x] ~~Coffee-hard questions and code;~~
- [x] ~~Yelp-hard questions and code;~~
- [x] Airbnb-hard questions and code;
- [x] ~~SciREX-hard questions and code;~~
- [x] ~~Agenda-hard questions and code;~~
- [x] ~~DBLP-hard questions and code;~~

### Benchmark Code Release
- [ ] ChatGPT Vanilla;
- [ ] Chain-of-Thoughts;
- [ ] ReAct;
- [ ] Chameleon;

