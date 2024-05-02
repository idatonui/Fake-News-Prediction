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

In today's digital landscape, the rampant spread of misinformation and fake news poses a grave threat to societies worldwide. With 68% of American adults relying on social media for news, falsehoods can easily proliferate unchecked, as evidenced by studies showing that false information on platforms like Twitter spreads faster and wider than truth. The consequences are dire, eroding trust in institutions, polarizing communities, and undermining democratic processes.

The impact of fake news extends beyond politics, significantly affecting public health. During the COVID-19 pandemic, misinformation led to confusion and panic-buying of unproven remedies, while vaccine hesitancy fueled by false claims jeopardized efforts to curb the virus's spread. Addressing this challenge requires data-driven approaches, drawing on techniques from machine learning, natural language processing, and social network analysis. Researchers and policymakers are increasingly leveraging these tools to predict and mitigate the dissemination of fake news, enabling targeted interventions to combat its harmful effects.


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




![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/Subjects%20in%20Fake%20News.png)




## Modeling
 Two models (Logistic Regression and ) were built and trained using the training dataset and CountVectorizer class from the sklearn library was used to convert the preprocessed text into feature vectors. Multinomial Naive Bayes Model and Support Vector Machine Model performance were used to compare it with the baseline model. The performance of the models was evaluated using accuracy, precision and recall.

## Model Evaluation

1. The baseline Logistic Regression model achieved exceptional performance across all metrics, with accuracy, precision, recall, and F1-score all exceeding 99%.
2. The Multinomial Naive Bayes model exhibited slightly lower performance compared to the baseline Logistic Regression model, with all metrics around 94.78%.
3. The Support Vector Machine model demonstrated similar performance to the baseline Logistic Regression model, with all metrics reaching approximately 99.36%.


- Both the baseline Logistic Regression and the Support Vector Machine models outperformed the Multinomial Naive Bayes model in terms of accuracy, precision, recall, and F1-score.
- Among these models, the Support Vector Machine model showed the most promising performance, matching or slightly surpassing the baseline Logistic Regression model across all metrics.
- Therefore, based on the provided evaluation results, the Support Vector Machine model appears to be the better-performing model for the task of classifying fake news articles, followed closely by the baseline Logistic Regression model.


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
