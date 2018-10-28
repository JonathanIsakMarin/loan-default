# Predicting loan default in peer-to-peer loan markets
In this project I have used methods machine learning models and Natural Language Processing to build predictive models, and test to which degree I can predict whether borrowers will default on their loans in peer-to-peer lending markets. I have used  data from one of the world’s largest P2P platforms, Lending Club. The data is publicly available on www.lendingclub.com

Peer-to-peer lending is a promising lending platform. Ordinary people can invest in giving loans to other people. It is like a form of crowd-sourcing where everyone can help each other out financially and gain a profit also! However, if people default on their loans it ruins the trust in the system which can deter people from using P2P-lending. Therefore, it is pretty interesting to see if we can find people who are likely to default before they actually default on their loans. This allows for preventive measures. 

### The data
This data contains a range of interesting variables about the borrowers receiving the loans as well as whether the borrowers have defaulted or not. It contains quantitative loan-level data, such as the loan amount, the interest rate of the loan, and the annual income of the borrower. Interestingly, it also contains text bits written by borrowers themselves. These loan descriptions serve as the borrower’s motivational letter for what he/she want to use the money for, and why he/she should be given it.  

The loan descriptions offer a very intersting way of incoporating text analysis into machine learning models. I try to predict the probability that borrowers default using the commonly provided loan-level data as well as their loan descriptions. 

### Results
I found the best performing models using a down-sampling procedure due to a high level of imbalance in the target variable (few people who default on their loans). Testing KNN, Random Forests and Logistic Regression yielded the following results. Not super impressive overall. And the models appear to perform very similar. Maybe you can do better? :-) You will also find some descriptive statistics in the notebook that are interesting.


|              | Accuracy       | Precision     | Recall      | F1        |
| :---         |  :---          |  :---         | :---        | :---      |
|KNN           | 0.62           | 0.23          | 0.63        | 0.33      |
|Random Forest | 0.61           | 0.22          | 0.59        | 0.32      |
|Logistic      | 0.62           | 0.23          | 0.64        | 0.34      |


