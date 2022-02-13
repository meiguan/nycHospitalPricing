# Are Healthcare Costs Predictable?
2019

Mei Guan <yg833@nyu.edu>
Qinyu Goh <qg412@nyu.edu>
Rachel Sim <rms818@nyu.edu> 

> [(WIP) Urban Health - A Case of New York State](https://docs.google.com/document/d/1E-6TzyWT64FEHilkx_iuYlyBxW69mx6EEtT-9xZ68sE/edit?usp=sharing)


### TL;DR

1. Mandate for all hospitals to publish master-charges in a machine readable format is a step in the right direction to promote pricing transparency. However, we believe there needs to be more work to standardize how master-charges are reported across healthcare providers. Currently, the discrepancies between how procedures are coded make it also impossible to make comparisons between providers--comparing one section procedure to another, it is hard to say if they are infact the same basket of goods. 

2. Using both random forest and decision tree models on the existing publicall available datasets from CMS and Health Data NY, the results were promising with above 80% accuracy for out of sample predictions.

3. For the different models, upwards of 50 features were fed into the models. And doing one-hot encoding on the categorical features then the resultant frame was over 150 columns. This was a curse of dimensionality. And in an effort to reduce the dimensions, PCA was employed, but did not improve model performance. Perhaps the next step is to LDA.

### Motivation for This Project
With cities becoming more populous and serving as the main catchment of people in the world by 2050 (World Health Organisation, 2019), urban health has become increasingly critical. There are 3 main aspects to urban health: the physical living conditions, the social environment as well as access to health and social services (Galea and Vlahov, 2005). Cities with good urban health reap a multitude of tangible and intangible benefits; a healthy city is defined to be one that sustainably provides resources for improving all aspects of the urban environment such that residents are able to engage in all functions of life and develop maximum potential (World Health Organisation, 2019). 

The impact of bad urban health can be dire. Researchers have concluded that the American economy is losing as much as $260 billion per year to health-related productivity losses (Mattke, Balakrishnan, Bergamo & Newberry, 2007). More specifically, the lack of access to affordable health services has resulted in 1 in 10 Americans not getting or delaying health care (Claxton, Sawyer & Cox, 2019). To quote John F Kerry on the American healthcare system - “The problem with the American healthcare system is that it is not working for the American family”. 

### Problem Statement

To reiterate, America’s major urban health problem lies in the fact that there is a lack of access to affordable health care. Healthcare is expensive due to price opacity and increasing price transparency is one potential solution that can help reduce the cost of healthcare in America. 

The goal of this project is therefore to answer this simple question of: What should a patient be expected to pay given that he or she knows what is their condition? This question is answered in the context of New York State, in three main segments using a series of machine learning algorithms that   Ordinary Least Square Regression (OLS), Principal Component Analysis (PCA) and Random Forest Regression (RFR):
Arthroplasty and C-Section Analysis
Top 10 Diagnosis Related Group (DRG) codes

By predicting total charges for each potential patient based on a set of curated variables, we are solving for a regression problem that can help inform the extent to which important features influence total charges. Meanwhile, the analysis of specific medical procedures such as Arthroplasty and C-Section provides the first glimpse of how the modelling of prices can be done for each specific medical condition and procedure. This is followed by a more macro approach of modelling total charge incurred based on 10 DRG codes, which is an attempt to see the feasibility of having one model based on a multitude of DRG codes instead of having to do one model for each DRG code. 
