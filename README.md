# Funding Campaign Success Predictor - Kickstarter

![Kickstarter_image](https://a.kickstarter.com/assets/site/social/og-kickstarter-social-new-d68ea5b8257b3ff7ec063993ddc0f9662494309832feb40117fc936fa1c819a2.png)

Authors: Tjade Appel & Felix Seeliger

This project is still **in progress**.  


## Overview 

Kickstarter is an American public benefit corporation based in Brooklyn, New York, that maintains a global crowdfunding platform focused on creativity. On this platform initiators can bring their ideas to a concrete project.

A lot of people contribute to these projects in form of donating money. These donators are called backers. Many of these backers support projects out of interest in the related topic, or out of sympathy with the initiator. As a reward for the support the backers, depending on the amount of money they contributed, receive a gift or the finished product itself.

Each project has a campaign time prior to the project itself that lasts up to 60 days. During this time the money needed to realize the project is collected. If not enough money is funded, the project is considered as not successful and none of the backers are charged. If the target amount is reached, the backers will be charged and the money is going to be transferred to the initiator, so he or she can start with the project itself.


## Business Case:  

A lot of backers ask themselves, if the project they're thinking of donating to is going to be successful. To contribute in an unsuccessful project doesn't mean to lose money, but it means to reserve money for a project, that can't be used for other purposes during the campaign time. It could be used for example for a project that has a better chance of being successful and is still looking for additional backers.

Given these thoughts, we had a closer look at the dataset at hand, providing the metadata for more than 200000 projects on kickstarter. We'll have a closer look at these observations in order to gather information that supports initiators to find out what the criteria for a succesful project are. Moreover, we will implement and evalutate different machine learning algorithms to support backers in making a decision, if it is worth to donate or not.


## Outcome / Findings:

Based on the tested models values of more than 85% for our goal metric (True Positive Rate) can easily be achieved. Nevertheless, if we only try to optimize this metric, the recall and the overall accuracy of our models will be diminished, since the model will predict less successful outcomes overall, resulting in a higher number of false negative predictions. This needs to be taken into account when choosing the model for your prediction.  

Based on these thoughts the best model, that we could find so far is a tuned Random Forest Model with a **precision** of **90%** and a **F1-Score** of **86.51%**.


## Contents of Repository
---

- Project 2 - Kickstarter Campaign Success Predictor.ipynb (main Jupyter Notebook)
- Project 2 - Kickstarter Presentation.pdf (presentation of findings)
- data (directory with the raw metadata)


## Python Modules Used:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Datetime
- Scikit Learn
 
## Future work

- implementing more features (maybe success rate of the creator of the campaign at hand)
- implementing different ensemble models like AdaBoost, XGBoost or StackingClassifier on the algorithms used
