# module-20---Initial-Report---EDA

 # Predictors of Startup Success 
### Introduction
A Startup is a new company (qualified when still at a project phase) which seeks to develop an innovation capable of disrupting sectors. While entrepreneurship refers to all new businesses, including self-employment and businesses that never intend to become registered, startups refer to new businesses that intend to grow and validate a scalable economic model.  

Startups play a major role in the economic growth of many countries. They bring new ideas, spur innovation, create new technologies and are an important source of employment. Over the past two decades, the startup sector has grown exponantially in number of new companies and in the volume of capital seeking to participate as investments.

Due to their high risks, startups face high uncertainty and a minority of them go on to be successful and influential. Their inherent risk and requirement for large amounts of capital make successful investment hard to come by. In fact, on average Venture Capital Funds (the main investors in startups) have a successful (IPO) investment rate of 1 out of 32. After adventuring myself in the field, it is clear that investors have limited tools to objectively identify the qualities of a successful startup and their potential to attain "success".  


Before we continue, it is important to define "what is a successfull startup?". Often we have in mind sotries of "IPO unicorns" like Facebook or Amazon, but in fact startup success could be generalized the realization of an "Exit". These events can be intiated by an acquisition (M&A) or an IPO (Initial Public Offering)

### Project Overview
Startup companiies are recently emerging and evolving more than ever. But still, many of them fail, in fact, 9 out of 10 startups fail. So, what are the characteristics of startups which succeed? There are many factors that might play a role in this question: founders and team experience, fundings, location, product, market and so on. Why some startups are acquired very early and others are not? Are ther maybe some factors that attract bigger companies into some startup acquisition? This report aims to investigate these questions using the [Startup Success Prediction](https://www.kaggle.com/datasets/manishkc06/startup-success-prediction) dataset available on Kaggle.  

### Problem Statement
The startup world requires a lot of decision making from the people involved, specially when dealing with situations of funding or acquisitions that will result in ownership changes. In these situations, the decision maker should have on hand all the information that can be provided with the amount of data available otday about companies, funding rounds and acquisitions.  

This project proposes a serie of supervised learning models that can forecast a startup success as well as a better understanding of the variables that most impact the acquisition or failure of a startup company. **Different supervised algorithms will be tested in order to compare our results and better understand the variables that most impact the outcome.**

### Performance Metrics
To evaluate the validity of each model we will use the True Positive Rate, False Positive Rate and the Area under the ROC Curve (AUC_ROC). True Positive rate and False Positive rates will derived from the confusion matrix of our classifiers. Since we expect the dataset to be imbalanced such metric wil be much more useful than accuracy. We expect the number of companies that are acquired will be much smaller than those in operation or closed. If we were to use accuracy, our models would probably have a high score even though their will be performing poorly of retrieving the few companies that are more likely to be acquired.  

The ROC curve combines TPR(y-axis) and FPR (x-axis). In general, the AUC is a good metric for binary classification problems.