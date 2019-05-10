# Machine Learning for Cities Group Project

## Working Title: Predicting Hospital Pricing
2019
Qinyu Goh <qg412@nyu.edu>
Mei Guan <yg833@nyu.edu>
Rachel Sim <rms818@nyu.edu> 

### TL;DR


### About This Project
With cities becoming more populous and serving as the main catchment of people in the world by 2050 (World Health Organisation, 2019), urban health has become increasingly critical. There are 3 main aspects to urban health: the physical living conditions, the social environment as well as access to health and social services (Galea and Vlahov, 2005). Cities with good urban health reap a multitude of tangible and intangible benefits; a healthy city is defined to be one that sustainably provides resources for improving all aspects of the urban environment such that residents are able to engage in all functions of life and develop maximum potential (World Health Organisation, 2019). 

The impact of bad urban health can be dire. Researchers have concluded that the American economy is losing as much as $260 billion per year to health-related productivity losses (Mattke, Balakrishnan, Bergamo & Newberry, 2007). More specifically, the lack of access to affordable health services has resulted in 1 in 10 Americans not getting or delaying health care (Claxton, Sawyer & Cox, 2019). To quote John F Kerry on the American healthcare system - “The problem with the American healthcare system is that it is not working for the American family”. 

### Problem Statement

To reiterate, America’s major urban health problem lies in the fact that there is a lack of access to affordable health care. Healthcare is expensive due to price opacity and increasing price transparency is one potential solution that can help reduce the cost of healthcare in America. 

The goal of this project is therefore to answer this simple question of: What should a patient be expected to pay given that he or she knows what is their condition? This question is answered in the context of New York State, in three main segments using a series of machine learning algorithms that   Ordinary Least Square Regression (OLS), Principal Component Analysis (PCA) and Random Forest Regression (RFR):
Arthroplasty and C-Section Analysis
Top 10 Diagnosis Related Group (DRG) codes

By predicting total charges for each potential patient based on a set of curated variables, we are solving for a regression problem that can help inform the extent to which important features influence total charges. Meanwhile, the analysis of specific medical procedures such as Arthroplasty and C-Section provides the first glimpse of how the modelling of prices can be done for each specific medical condition and procedure. This is followed by a more macro approach of modelling total charge incurred based on 10 DRG codes, which is an attempt to see the feasibility of having one model based on a multitude of DRG codes instead of having to do one model for each DRG code. 
