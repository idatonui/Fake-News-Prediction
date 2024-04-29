# **Fake News Detection**


## Authors

1. Ida Chepng'eno
2. George Mbugua
3. Kevan Ndwiga
4. Daniel Muruthi
5. Mike Kiptoch
6. Neville Ngenzi



## 1. **BUSINESS UNDERSTANDING**

As a leading news organization in Kenya, Tuko News faces the formidable challenge of combating fake news to uphold journalistic integrity and maintain public trust. The dissemination of fake news poses substantial risks to Tuko News, including erosion of reader confidence, polarization of public opinion, and potential legal ramifications. To address these challenges, Tuko News recognizes the urgent need for sophisticated systems capable of detecting and flagging fake news in real-time. By implementing robust fake news detection mechanisms, Tuko News aims to safeguard its reputation, enhance public trust, and ensure the dissemination of accurate and reliable information.


### a. Introduction

In today's digital age, the spread of misinformation, commonly known as fake news, has become a pervasive issue, undermining the integrity of journalistic organizations worldwide. Tuko News, as a leading news organization in Kenya, recognizes the gravity of this challenge and aims to address it proactively. Through the implementation of advanced technologies and rigorous methodologies, Tuko News seeks to combat the dissemination of fake news and uphold its commitment to journalistic integrity and public trust.

### b. Problem Statement

#### **What is the prevailing Circumstance?**

The proliferation of social media platforms and digital news outlets has facilitated the rapid dissemination of information, both accurate and false. This unprecedented accessibility to news sources has led to an alarming increase in the circulation of fake news, which poses significant risks to Tuko News and its stakeholders.

#### **What problem is being addressed?**

The primary problem being addressed is the pervasive presence of fake news within the digital media landscape. Fake news undermines the credibility of Tuko News as a reputable journalistic entity, erodes reader confidence, and contributes to the polarization of public opinion. Moreover, the dissemination of false information can have far-reaching consequences, including social unrest, political instability, and legal ramifications.

#### **How the project aims to solve the problems?**

The project aims to develop and implement sophisticated systems for detecting and flagging fake news in real-time. By leveraging cutting-edge technologies such as natural language processing (NLP), machine learning (ML), and data analytics, Tuko News intends to identify and verify the authenticity of news articles and sources. Additionally, the project will involve the establishment of rigorous editorial standards and fact-checking procedures to ensure the dissemination of accurate and reliable information to its audience. Through these initiatives, Tuko News seeks to safeguard its reputation, enhance public trust, and uphold the principles of ethical journalism.



### c. Objectives

#### Main Objectives

- To implement robust fake news detection mechanisms capable of identifying and flagging misinformation in real-time, thereby safeguarding the integrity and credibility of Tuko News.

#### Specific Objectives

1. Develop a comprehensive dataset of labeled news articles, encompassing both genuine and fake content, to train and validate machine learning models for fake news detection.
2. Utilize natural language processing (NLP) techniques to extract relevant features from news articles, such as linguistic patterns, sentiment analysis, and lexical semantics.
3. Implement state-of-the-art machine learning algorithms, including supervised and unsupervised learning approaches, to classify news articles as genuine or fake based on extracted features.
4. Integrate the fake news detection system seamlessly into Tuko News's content management workflow, enabling automated flagging and verification of potentially false information.
5. Establish a framework for continuous monitoring and evaluation of the fake news detection system's performance, including metrics such as precision, recall, and F1 score.
6. Conduct regular updates and improvements to the fake news detection system to adapt to evolving misinformation tactics and enhance its accuracy and reliability over time.


### d. Notebook Structure

i. Business Understanding
ii. Data Understanding
iii. Exploratory Data Analysis
iv. Data Preprocessing
v. Modeling
vi. Evaluation
vii. Conclusion
viii. Recommendation
ix. Next Steps


### e. Stakeholders

The media sector, news organizations, and social media sites that disseminate news pieces can all benefit from this endeavor. These organizations can enhance their content control and stop the spread of false information by categorizing news stories as legitimate or fake.


### f. Metric of Success

- The performance of the model is evaluated based on achieving an accuracy of over 85%.


## 2. **Data Understanding**

The dataset comprises two CSV files: "Fake.csv" and "True.csv", sourced from Kaggle each contain 20,000 rows. Columns include 'title', 'text', 'subject', and 'date'
Each file contains news articles, distinguished by their authenticity. 'Fake.csv' contains fake news articles, while 'True.csv' contains genuine news articles.


Title Column:
Offers succinct summaries of news article content.
Crucial for headline analysis and understanding key themes. 
Text Column:
Contains full textual content of the news articles.
Provides detailed information for NLP tasks such as sentiment analysis and text classification. 
Subject Column:
Categorizes news articles into specific subjects or domains.
Enables filtering and analysis based on topics of interest.
Date Column:
Records publication dates of news articles.
Facilitates temporal analysis and trend tracking.


## Data Visualization & Preprocessing

### EDA

- This stage entails thoroughly exploring and comprehending the dataset prior to employing machine learning algorithms. It plays a crucial role in tasks such as data preprocessing, selecting appropriate models, and devising strategies for evaluating model performance.

#### Distribution of Subject Column

This is the distribution of subjects within the true news dataset using a bar plot, providing insights into the variety and frequency of different subjects covered in the news articles.


![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/subject%20in%20True%20News.png)


- This bar plot illustrate the distribution of subjects in both true and fake news datasets. This can help identify which subjects are more common in each dataset and whether there's a notable difference.



![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/subject%20in%20True%20News.png)


The bar chart shows the distribution of subjects covered in true news articles, with politics being the most common subject and world news following in second.  



### Visualization: Word Clouds


- This segment provides a visual representation of the most frequent words in both true and fake news datasets through word clouds, allowing for quick insights into the prevalent themes or topics within each category.

#### Fake News Word Cloud


![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/Word%20Cloud%20for%20Fake%20News.png)


#### True News Word Cloud


![Alternative text](https://github.com/idatonui/Fake-News-Prediction/blob/main/images/word%20cloud%20for%20True%20News.png)



## Modeling
 
### Baseline Model: Logistic Regression

The baseline model serves as an initial benchmark for evaluating the performance of more complex models in the task of fake news prediction. In this project, logistic regression is employed as the baseline model.

Below are the performance metrics derived from the model evaluation:
- Accuracy: 99.53%
- Precision: 99.67%
- Recall: 99.35%
- F1 Score: 99.51%

Interpretation of Metrics
- Accuracy: Indicates the overall correctness of predictions, with our model achieving an accuracy of 99.53%.
- Precision: Reflects the reliability of our model in correctly identifying fake news articles, with a precision score of 99.67%, minimizing false positives.
- Recall: Measures the model's ability to capture all actual instances of fake news, achieving a recall score of 99.35%, thus reducing false negatives.
- F1 Score: Represents the harmonic mean of precision and recall, indicating a balanced performance between the two metrics, with our model achieving an F1 score of 99.51%.


The baseline Logistic Regression model demonstrates exceptional performance in accurately classifying fake news articles. However, further evaluation on unseen data and exploration of advanced models may be warranted to ensure robustness and generalization.


### Improving the Performance of the Model

While logistic regression model performed well on the test set, there are ways to make it even more efficient:

- **Feature engineering:** Using more complex text representations, such as word embeddings or topic models, in place of merely using a bag-of-words approach, may help reveal more detailed relationships between words.

- **Hyperparameter optimization:** this will determine the best parameter configuration for the dataset by fine-tuning the logistic regression model's hyperparameters using strategies like grid search and randomized search.

**Multinomial Naive Bayes Model**

Performance Metrics:

Accuracy: 94.78%
Precision: 94.78%
Recall: 94.78%
F1-score: 94.77%


**Support Vector Machine Model**
Performance Metrics:

Accuracy: 99.36%
Precision: 99.36%
Recall: 99.36%
F1-score: 99.36%


Both models were trained and evaluated for the task of classifying fake news articles. The Multinomial Naive Bayes model achieved an accuracy, precision, recall, and F1-score of approximately 94.78%. Meanwhile, the Support Vector Machine model exhibited superior performance with all metrics reaching approximately 99.36%.

The Support Vector Machine model demonstrated higher accuracy and precision compared to the Multinomial Naive Bayes model, indicating its effectiveness in accurately classifying fake news. However, further analysis and fine-tuning may be necessary to optimize both models for specific project requirements.



### Model 2: Deep Learning with Convolutional Neural Networks (CNNs)

- Using 1D convolutions to extract patterns (like n-grams) in the text.


### Model Evaluation
