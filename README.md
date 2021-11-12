# BT4012 Final Project Repository

## Investigating 3 types of Fraud Detection Methods in Detecting Credit Card Fraud

## Authors:

**Group 31**
- Loh Hong Tak Edmund (A0199943H)
- Tan Yi Bing (A0204181U)
- Yap Hui Yi (A0203707M)

## Table of Contents
1. [Authors](#authors)
2. [About the Project](#about-the-project)
3. [Codes and Resources Used](#codes-and-resources-used)
4. [Getting Started](#getting-started)
5. [Acknowledgements](#acknowledgements)

## About the Project

In this project, we aim to explore different fraud detection models in case of credit card fraud transactions. Hence, we have chosen 3 research papers that have proposed machine learning models in this field to tackle this problem.

The 3 papers chosen are as follows:
1. Sequence classification for credit-card fraud detection
    The paper phrased the fraud detection problem as a sequence classification task using LSTMs and compared with a RandomForest Classifier
2. AI2: Training a big data machine to defend
    The AI2 system combines four main components - a big data behavioural analytics platform, an ensemble of outlier detection methods, an analyst feedback mechanism and a supervised learning module, to detect fraudulent transactions.
3. FraudMiner: A Novel Credit Card Fraud Detection Model Based on Frequent Itemset Mining 
    FraudMiner first constructs a pattern database using Frequent Itemset Mining to form legal and fraud patterns of each customer. The model then classifies incoming transactions by comparing them with the pattern databases.
    
For each research paper, we did an implementation of the proposed model using [Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/kartik2112/fraud-detection) and evaluated their performance on the dataset.

This dataset is simulated by [Sparkov Data Generation](https://github.com/namebrandon/Sparkov_Data_Generation), and it covers credit cards of 1000 customers doing transactions with a pool of 800 merchants.

## Methodology

1. We have implemented the respective proposed algorithms in simplified models. 
2. We trained and tested the models on the Credit Card Fraud Detection dataset. 
3. We compared the three different models using the metrics F2-Score, Precision and Recall, to determine which model can most effectively detect fraudulent transactions.
        a. F2-Score is used as it emphasises minimising False Negatives (Lee, 2020), which is costly in fraud detection. 
![equation](https://latex.codecogs.com/svg.image?\bg_white&space;F2&space;Score&space;=&space;\frac{(1&plus;2^{2})*Precision*Recall}{2^2&space;*&space;Precision&space;&plus;&space;Recall})
4. We mined for insights through our comparisons and identified assumptions and potential limitations in our simplified implementations.


## Results

| Model                                     | F2-Score      | Precision  | Recall     |
| -------------                             | ------------- | ---------- | ---------- | 
| FraudMiner                                | 0.712098      | 0.367589   | 0.930000   |
| LSTM + RandomForest Feature Selection     | 0.653061      | 0.780488   | 0.784314   |
| AI2 (after 15 timesteps)                  | 0.509356      | 0.671233   | 0.480392   |
| Baseline RandomForest                     | 0.206767      | 1.000000   | 0.215686   |


## Codes and Resources Used

**Python Version:** 3.9.5

**Built with:** Jupyter Notebook

**Packages:** pandas, numpy, matplotlib, collections, seaborn, imblearn, sklearn, tensorflow, keras, warnings, apyori, gc

**Data Set:** [Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/kartik2112/fraud-detection)

## Getting Started

### Prerequisites

Make sure you have installed all of the following prerequisites on your development machine:
- Python 3.9.5
- Jupyter Notebook 6.4.4

### Installation

The requirements.txt file contains Python libraries that your notebooks depend on, and they will be installed using:

```pip install -r requirements.txt```


## Acknowledgements

We would like to express thanks to the authors of the papers we have selected. 

For [Sequence classification for credit-card fraud detection](https://doi.org/10.1016/j.eswa.2018.01.037),

  *Johannes Jurgovsky, Michael Granitzer, Konstantin Ziegler, Sylvie Calabretto, Pierre-Edouard Portier, LiyunHe-Guelton, Olivier Caelen* 

For [AI2: Training a big data machine to defend](https://doi.org/10.1109/BigDataSecurity-HPSC-IDS.2016.79),

  *Kalyan Veeramachaneni, Ignacio Arnaldo,Alfredo Cuesta-Infante, Vamsi Korrapati, Costas Bassias, Ke Li*

For [FraudMiner: A Novel Credit Card Fraud Detection Model Based on Frequent Itemset Mining](https://doi.org/10.1155/2014/252797),

  *K. R. Seeja and Masoumeh Zareapoor*

We would also like to thank Kartik Shenoy, the owner of the  [Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/kartik2112/fraud-detection), for allowing usage of the dataset. 







