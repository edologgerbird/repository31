# BT4012 Group 31 Final Project Repository

## Authors:
- Loh Hong Tak Edmund (A0199943H)
- Tan Yi Bing (A0204181U)
- Yap Hui Yi (A0203707M)


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

The requirements.txt file should lists Python libraries that your notebooks depend on, and they will be installed using:

```pip install -r requirements.txt```


## Table of Contents

## Abount the Project

In this project, we aim to explore different fraud detection models in case of credit card fraud transactions. Hence, we have chosen 3 research papers that have proposed machine learning models in this field to tackle this problem.

The 3 papers chosen are as follows:
1. Sequence classification for credit-card fraud detection
    The paper phrased the fraud detection problem as a sequence classification task using LSTMs and compared with a RandomForest Classifier
2. AI2: Training a big data machine to defend
    The AI2 system combines four main components - a big data behavioural analytics platform, an ensemble of outlier detection methods, an analyst feedback mechanism and a supervised learning module, to detect fraudulent transactions.
3. FraudMiner: A Novel Credit Card Fraud Detection Model Based on Frequent Itemset Mining 
    FraudMiner first constructs a pattern database using Frequent Itemset Mining to form legal and fraud patterns of each customer. The model then classifies incoming transactions by comparing them with the pattern databases.
    
For each research paper, we did an implementation of the proposed model using Credit Card Transactions Fraud Detection Dataset and evaluated their performance on the dataset.

This dataset is simulated by [Sparkov Data Generation](https://github.com/namebrandon/Sparkov_Data_Generation), and it covers credit cards of 1000 customers doing transactions with a pool of 800 merchants.

## Acknowledgements

We would like to express thanks to the authors of the papers we have selected. 

For [Sequence classification for credit-card fraud detection](https://doi.org/10.1016/j.eswa.2018.01.037),

  *Johannes Jurgovsky, Michael Granitzer, Konstantin Ziegler, Sylvie Calabretto, Pierre-Edouard Portier, LiyunHe-Guelton, Olivier Caelen* 

For [AI2: Training a big data machine to defend](https://doi.org/10.1109/BigDataSecurity-HPSC-IDS.2016.79),

  *Kalyan Veeramachaneni, Ignacio Arnaldo,Alfredo Cuesta-Infante, Vamsi Korrapati, Costas Bassias, Ke Li*

For [FraudMiner: A Novel Credit Card Fraud Detection Model Based on Frequent Itemset Mining](https://doi.org/10.1155/2014/252797),

  *K. R. Seeja and Masoumeh Zareapoor*

We would also like to thank Kartik Shenoy, the owner of the  [Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/kartik2112/fraud-detection), for allowing usage of the dataset. 







