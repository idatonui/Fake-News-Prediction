![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/how-to-identify-fake-news-1.jpg)


# **Fake News Detection**


## Authors

1. Ida Chepng'eno
2. George Mbugua
3. Kevan Ndwiga
4. Daniel Muruthi
5. Mike Kiptoch
6. Neville Ngenzi



## Introduction

In today's digital age, the spread of misinformation, commonly known as fake news, has become a pervasive issue, undermining the integrity of journalistic organizations worldwide. The impact of fake news extends beyond politics, significantly affecting public health. During the COVID-19 pandemic, misinformation led to confusion and panic-buying of unproven remedies, while vaccine hesitancy fueled by false claims jeopardized efforts to curb the virus's spread. Addressing this challenge requires data-driven approaches, drawing on techniques from machine learning, natural language processing, and social network analysis. Researchers and policymakers are increasingly leveraging these tools to predict and mitigate the dissemination of fake news, enabling targeted interventions to combat its harmful effects.


## Problem Statement

The primary problem being addressed is the pervasive presence of fake news within the digital media landscape. Fake news undermines the credibility of International News as a reputable journalistic entity, erodes reader confidence, and contributes to the polarization of public opinion. Moreover, the dissemination of false information can have far-reaching consequences, including social unrest, political instability, and legal ramifications.


## Main Objectives

- To implement robust fake news detection mechanisms capable of identifying and flagging misinformation in real-time, thereby safeguarding the integrity and credibility of most News sectors.


## Data Understanding

The data used in this project was obtained from: [Kaggle](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset). The dataset is divided into: Fake.csv and True.csv.

The Fake.csv file contains: 23481 rows and 4 columns

The True.csv file contains: 21417 rows and 4 columns



## Data Preparation

This involves cleaning, addressing missing values, and removing duplicates to ensure data accuracy and completeness for analysis and modeling. Exploratory Data Analysis was done to understand data relationships, patterns, and distributions, guiding model selection and hyperparameter tuning.

Text preprocessing was also performed and it involved steps like lowercasing, removing punctuation and digits, eliminating stop words, and either stemming or lemmatizing text. These steps aim to streamline text data for model training by reducing complexity and focusing on essential words, although they may result in some loss of information.


#### Distribution of Subject Column



![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/subject%20in%20True%20News.png)




![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/Subjects%20in%20Fake%20Class.png)




## Modeling
 Two models (Logistic Regression and LSTM) were built and trained using the training dataset and CountVectorizer class from the sklearn library was used to convert the preprocessed text into feature vectors. LSTM model was also tuned and the results were compared with the two models. The performance of the models was evaluated using accuracy.

## Model Evaluation

- Logistic Regression:
Accuracy: 99.53% (highest among the three models).
- LSTM:
Accuracy: 98.48% (second highest).
- Tuned LSTM:
Accuracy: 98.46% (slightly lower than Basic LSTM).


- Logistic Regression performed the best in terms of accuracy.
- Basic LSTM and Tuned LSTM showed comparable results with slight variations.
- Results suggest that traditional models like Logistic Regression can be more accurate than deep learning models in some cases.

Logistic Regression, with a 99.53% accuracy rate, stands out as the best model for fake news detection among the evaluated models. Its high accuracy allows for precise identification and flagging of fake news, reducing false positives and negatives. By analyzing text-based features, Logistic Regression can quickly and effectively classify news articles as real or fake, making it a reliable choice for combating misinformation in real-time scenarios. This accuracy ensures robust content filtering and helps maintain information integrity.


## Limitations and Next Steps


### Limitations

While the project has made significant strides in fake news detection, several limitations must be acknowledged. Firstly, the dataset used for training and evaluation primarily consists of news articles from the United States, predominantly focusing on political subjects. This inherent bias in the data may limit the generalizability of the models to other regions or topics. Moreover, the dataset size, while substantial, may not encompass the full spectrum of fake news characteristics, potentially leading to model overfitting or underperformance on unseen data. Additionally, the preprocessing techniques applied to the text data, such as stemming or lemmatization, may inadvertently remove context or nuance crucial for accurate classification. 



### Next Steps:

- Diversification of Dataset: Expand the dataset to include news articles from diverse geographical regions, languages, and subject matters. This broader dataset will provide a more comprehensive understanding of fake news characteristics across different contexts, enhancing model generalization.

- Fine-Tuning Preprocessing Techniques: Evaluate and refine text preprocessing techniques to preserve essential context and semantics while still reducing noise and complexity. Experiment with alternative methods such as contextual embeddings or transformer-based architectures to capture richer linguistic features.



## Recommendation

1. Education and Media Literacy Initiatives: Launch educational campaigns and media literacy initiatives to empower individuals with the skills and knowledge to critically evaluate information sources and discern fact from fiction. Promote digital literacy skills among vulnerable populations, including students, seniors, and marginalized communities.

2. Partnerships with Tech Companies and Platforms: Forge partnerships with technology companies and social media platforms to deploy fake news detection tools and algorithms at scale. Collaborate on initiatives to curb the spread of misinformation and promote algorithmic transparency and accountability.

3. Continuous Evaluation and Improvement: Establish mechanisms for continuous evaluation and improvement of fake news detection systems. Solicit feedback from users, stakeholders, and subject matter experts to identify areas for enhancement and refinement.

4. Regulatory and Policy Interventions: Advocate for regulatory and policy interventions to address the proliferation of fake news and misinformation online. Engage with policymakers, regulatory bodies, and civil society organizations to develop evidence-based policies and regulations that safeguard information integrity and promote digital trust.

5. Investment in Research and Development: Allocate resources towards ongoing research and development efforts aimed at advancing fake news detection technologies. Foster interdisciplinary collaborations and partnerships to leverage expertise from diverse fields such as data science, linguistics, psychology, and journalism.
