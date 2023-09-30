<div align="center">
<h1> Natural Language Processing Project </h1>

[![projectReq](https://img.shields.io/badge/README-in_Polish-red)](https://github.com/s18579/ZUM_NLP/blob/main/README.pl-PL.md)
<a href="https://colab.research.google.com/drive/1Vs4Diav8Nqztfm7moZ6L8wPpStyI1UrR?usp=sharing" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

</div>


The Natural Language Processing (NLP) project carried out as the final project for the ZUM course aims to create a sentiment analysis model based on tweets from [Twitter/X](https://twitter.com/) related to current events in the world, in this case sentiment analysis about King Charles III from the period from September 1, 2022 (from the death of Queen Elizabeth II) to May 31, 2023 (coronation of Charles III).

Project was created as Jupyter notebook `.ipynb` in [Google Colab](https://colab.research.google.com/drive/1Vs4Diav8Nqztfm7moZ6L8wPpStyI1UrR?usp=sharing).

## Setup
The entire project was organized so that each stage could be run separately in the Google Colab environment. For each stage, the appropriate libraries are required, which are installed at the beginning of each stage. This makes the project flexible and easy to replicate in different environments.

In case of using a given notebook on a local IDE, it is recommended to install the data libraries contained in each section in the `Instalacja bibliotek` subsection in notebook.

### Stage 1: Data Collection
${\textsf{\color{red}This step may be obsolete due to Twitter/X ended free access to its API in Feburary 9, 2023. }}$

In this stage, using the `snscrape` lib, 22.5 thousand tweets were collected about King Charles III of Great Britain, collecting data from the period from September 1, 2022 (from the death of Queen Elizabeth II) to May 31, 2023 (coronation of Charles III). This process involved installing the necessary libraries, importing libraries, collecting data from Twitter, and then saving this data to a CSV file. Then, the data was cleaned and prepared for further analysis. This was done using custom-made data cleaning functions.

### Etap 2: Classic ML
The second stage focused on applying classic machine learning techniques to predict sentiment. Several algorithms were used here, including Naive Bayes, Logistic Regression and Decision Trees. Each of these models was properly trained and visualized to understand its effectiveness and results.

### Etap 3: Neural Model
At this stage of the project, a BLSTM model was used. After installing and importing the necessary libraries, the data was prepared for processing by the neural network. Then the model was trained and also fine-tuned to achieve the best result (in this case almost 90% accuracy on the test data set), visualized and tested.

### Etap 4: Language Model
The last stage focused on applying a language model, specifically DistilBERT, one of the Transformer BERT models. Preparing data for this model was similar to stage 3, but took into account the specifics of the BERT model. The model was then trained and tested to assess its effectiveness in analyzing tweet sentiment.

