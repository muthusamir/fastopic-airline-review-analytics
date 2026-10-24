FASTopic for Airline Customer Review Analytics

Topic Coherence, Diversity, and Longitudinal Insights

Overview

This repository contains source code and documentation for applying FASTopic to British Airways customer reviews. The study identifies recurring themes in passenger feedback, qualitatively compares the resulting topic structures with BERTopic, and examines quarterly topic-weight variation over time.

The analysis covers the period from 2014Q2 to 2023Q1 and focuses on exploratory customer-feedback analytics rather than causal inference or direct measurement of passenger satisfaction.

Research Objectives

Identify recurring themes in British Airways customer reviews using FASTopic.

Examine topic coherence, diversity, and potential topic redundancy.

Qualitatively compare the topic structures produced by FASTopic and BERTopic.

Describe quarterly topic-weight variation across pre-pandemic, pandemic, and recovery periods.

Document methodological considerations for reproducible topic-model evaluation.

Dataset

The study uses the Airways Customer Data dataset available from Kaggle.

Dataset: https://www.kaggle.com/datasets/ghassenkhaled/airways-customer-data/data

The cleaned corpus used in the reported analysis contains 3,397 unique review texts after deduplication.

Please obtain the dataset from its original source and comply with its licence and usage conditions. The dataset is not redistributed in this repository unless permitted by the applicable terms.

Models

FASTopic

The original analysis uses an eight-topic configuration ((K=8)) to identify themes relating to operational disruption, baggage and check-in, lounge facilities, seating and catering, crew service, cabin comfort, cabin class, and critical evaluations of food and staff.

A separate ten-topic FASTopic evaluation was conducted for additional diagnostic analysis. Its results are distinct from those of the original eight-topic configuration.

BERTopic

BERTopic was used as a comparison model. The reported analysis produced three broad topics. The comparison focuses on observed topic structures and does not establish general algorithmic superiority.

Evaluation

The study considers the following measures:

UCI topic coherence

NPMI topic coherence

Topic diversity

Top-term overlap using Jaccard similarity

Document–topic correlation

Quarterly mean topic weights

The evaluation settings and model configurations should be documented alongside the corresponding code. Results from different model configurations should not be treated as directly comparable unless the evaluation protocol is consistent.
