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

