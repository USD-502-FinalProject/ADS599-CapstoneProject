# ADS599-CapstoneProject

# Abstract
This study develops an effective method for sentiment analysis of user-generated content on drug review websites.
An ensemble of models is developed in order to accurately model the complexities of user- generated drug reviews.  A word-level, two- to three- word phrase and clause-level sentiment analysis algorithm is developed to capture such complexities including drug name, side effects, dosage, and drug taker’s health profile.  The method utilizes the hybrid approach to sentiment analysis – rule-based as well as automatic systems. 
Experiment results with 2,700 clauses show the effectiveness of the proposed approach, and it performed significantly better than the baseline approaches using a machine learning approach. Various challenging issues were identified and discussed through error analysis. The application of the proposed sentiment analysis approach will be useful not only for patients and their caretakers but also for physicians and researchers obtain valuable summaries of public opinion and “wisdom of the crowd” aggregation of drug review data. Since sentiment analysis is domain specific, domain knowledge in drug reviews is incorporated into the sentiment analysis algorithm to provide more accurate analysis. In particular, MetaMap is used to map various health and medical terms (such as disease and drug names) to semantic types in the Unified Medical Language System (UMLS) Semantic Network

# Business Background
The advent of the internet, as well as mobile applications, smart phones, and increased accessibility to cloud-based computing has ushered in an era of unprecedented levels of user-generated data that is ripe with valuable insights yet to be extracted.  About 3.95 billion pharmaceutical drugs are prescribed each year in the United States alone.  Drugs.com alone contains reviews for over 24,000 pharmaceutical drugs.  But do members of the public have access to tools and applications that can extract actionable insights from the plethora of user-generated drug reviews in order to make well-informed decisions on the drugs they are being prescribed?  A comprehensive offering of tools and applications is needed to make insights into this data and the accuracy of such available for public use.
While much research has been conducted for sentiment analyzers in the domain of business data like product reviews, the amount of research has been underwhelming in terms of drug reviews, of which the text resides in its own domain and would require its own specific sentiment analysis methods in order to be effective.  
The purpose of this paper is to develop an effective method for predicting the expected outcomes of a particular drug based on a user’s health profile.  This method will consist of an ensemble of predictive models including sentiment analyzers at the word, two- to three-word phrase and clause-level as well as prediction algorithms based on input parameters from the user-generated drug reviews.  These include dosage, brand or generic drug, side effects, and sentiment or opinion.  In terms of the drug taker’s health profile, these may include age, ethnicity, demographics, genetic predisposition, alcoholism, smoking, exercise regimen, sexual orientation, sleeping schedules, other comorbidities, diet makeup, occupation, living environment, mental health etc.  These may affect a drug taker’s ability to metabolize the drug and thus affect the expressions of side effects from a particular drug.
The methods utilized in this research paper will consist of a combination of sentiment analysis and an ensemble of predictive algorithms.  Sentiment analysis is a specific approach to natural language processing in which the opinion or emotional tone of a body of text is mined by specific best practice methods.  In conjunction with the other inputs, an ensemble model will be developed in order to accurately model all of the possible facets of inputs that contribute to the outcome of the drug review sentiment and various drug outputs (side effects, dosages, patient health profile).
therefore, MetaMap (Aronson & Lang, 2010) is used to map various health and medical terms (e.g., disease, symptom, and drug names) in the review documents to semantic types in the Unified Medical Language System (UMLS) Semantic Network, and the tagged semantic information is utilized for sentiment analysis.
We conducted a preliminary study where a clause-level sentiment classification algorithm was developed and applied to drug reviews on a discussion forum (Na et al., 2012). This study is based on our previous work, and we have improved the approach by adding additional rules for both handling more complex relations among words and utilizing domain
In the following sections, related work is described rst. en our sentiment analysis method is proposed, and its experiment results and issues are described and discussed. Finally, conclusion information is provided.

Much of the research on the sentiment analysis of drug reviews centers around predicting the general drug rating, binary or multi-class sentiment classification in reaction to taking a drug or the multi-class severity of the side effects.
Sentiment analysis employs the use of machine learning and natural language processing (NLP) to identify the emotion behind a body of text.  The two main approaches are rule-based or automated sentiment analysis, or a third being a hybrid of the two.  The rule-based includes NLP techniques such as tokenization, stemming, lexicons and parsing.  The second approach involves machine learning techniques which learn from the word and the order of the words.  Hybrid approach consists of both approaches and generally yields higher accuracy but requires more computational power and time to develop.
In terms of data preprocessing, various approaches have also been taken including natural language processing techniques where the text was broken down into word, clause, sentence and document levels.
In terms of models, approaches included the traditional machine learning models and deep learning classifiers of which the second outperformed by significant margin.  Of the machine learning models, random forest trained on count vectorizer outperformed other ML models.  Bidirectional LSTM (Bi-LSTM) model trained on GloVe embedding resulted in an even better accuracy and F1 score.  In recent years, the most popular approach has been with DL models which employ the generation of neural network like structures to perform computations and classification tasks.  A combination of three deep learning models in conjunction with a traditional model beat out traditional models by 2% in terms of accuracy and F1-measure.
Based on the results of past research, the conclusion is that a combination of models – both deep learning classifiers and machine learning classifiers is necessary in order to accurately model the side effects and outcomes of taking a certain drug.


# Problem Statement
The purpose of this paper is to endeavor to solve these missing pieces in the hope that it will lead to offering tools and applications that make drug reviews as useful insights that are accessible to the public.


# Summary of Findings



# Business Questions
How can this model be applied to real world scenarios and bring value busines wise?  The model can be deployed as a service to any drug taker who wants to perform a search on a particular drug.

So the questions should be how big is this market?  At what price are users willing to pay for this?  Are there different business models for this application of the predictive model?  Which one is the most viable with the largest ROI?


# Scope of analysis
Due to this being a limited time project of 7 weeks, the scope was limited to just warfarin and coumadin drug reviews on the druglib.com website.


# Approach
Approach is to use an ensemble model which tends to yield better performing results.  We sift through each drug review and mark a record based on whether it contained text for a particular side effect.  Side effects were kept in a dictionary to be checked against.


# Limitations
We are limited to the side effects covered in the dictionary and could potentially miss very rare side effects that may be telling of what a patient could potentially experience taking this drug.  We are limited as to how well the 


# Solution details
A predictive model was built using XGBoost ensemble model.  The features were derived based on the review text.  There was much information that could be drawn from this body of text so the model performed pretty well.  Side effects were easily predicted based on those inputs.


# Concluding summary
The model performed half decently overall.  But being in less than 80% for the F1 score, there is still a lot of room for improvement.


# Call to action (CTA)
There is a great need to make this information available to the public so that they can easily research and become aware of the potential side effects of the drugs that they are taking.

[Presentation]([https://youtu.be/P_fBrbRDses?feature=shared](https://youtu.be/XiNCTJHbCnQ))
