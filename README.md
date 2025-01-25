## Twitter Account Classification Using Account Metadata: <br/> Organization vs. Individual
[https://dx.doi.org/10.55730/1300-0632.3856](https://dx.doi.org/10.55730/1300-0632.3856)

#### Abstract
Organizations present their existence on social media to gain followers and reach out to the crowds. 
For social media related tasks and applications, such as social media graph construction, sentiment analysis and bot detection, 
it is required to identify the entities' account types. Some of the applications focus on personal accounts, whereas others need 
only non-personal accounts. This paper addresses the account classification problem by using minimum amount of data, namely using 
only account’s profile metadata. The proposed approach classifies accounts either as *organization* or *individual* without 
collecting tweet data of these accounts in a language-independent manner. The model uses a Long Short Term Memory (LSTM) 
network for processing the textual properties and a fully-connected neural network for processing the numerical features.
We apply our solution on a collection of Twitter accounts, as it is one of the most widely used social networks. 
Our classifier, which is based solely on the account metadata, achieves an average of 97.4 % accuracy under 7-fold cross-validation.
The experiments show that the account metadata is a qualified resource for a very accurate estimation of the account types.

#### Datasets 

You can find all datasets mentioned in the paper from [here](https://github.com/tweetpie/twitter-account-classification/tree/main/datasets). Each model is applied on different versions of the datasets, such as the Humanizr model applied on the balanced, unbalanced, and full version of the Humanizr dataset. The balanced version of the data set includes equal number of individual and organization accounts. The number of accounts is accomplished by undersampling the majority class. 

   
|Dataset Name   |      Number of Original Accounts      |  Number of Collected Accounts | Collection Percent |
|:----------|:-------------:|------:|------:|
| Humanizr |  18,922 | 17,790 | 94 %      |
| Demographer | 227,277 |  214,236 | 94 %    |

##### Table: Humanizr and Demographer dataset statistics.

The collected Humanizr dataset consists of 17,790 user accounts, in which 16,012 of them are labeled as individuals, 
and 1,778 of them are labeled as organizations. In the Demographer dataset, there are 214,236 accounts in which 185,224 
are labeled as individuals, and 29,012 are labeled as an organization. Since the Demographer dataset comprises the Humanizr dataset, 
the figures are based on the Demographer dataset. 

#### Notebooks

##### Interactive Data Analysis

[This notebook](https://colab.research.google.com/github/tweetpie/twitter-account-classification/blob/main/notebooks/InteractiveDataAnalysis.ipynb) contains interactive plots to visualize Followers-Following, Followers-Tweets, Followers-Likes, Tweets-Likes and Tweets-Media relationships.

##### Interactive Demo

[This notebook](https://colab.research.google.com/github/tweetpie/twitter-account-classification/blob/main/notebooks/InteractiveAccountTypeClassification.ipynb) provides an interactive service that predict the given Twitter account's label.

## Citation

```bibtex
@article{cetinkaya2022twitter,
  title={Twitter account classification using account metadata: organizationvs. individual},
  author={Cetinkaya, Yusuf Mucahit and G{\"u}rlek, Mesut and Toroslu, Ismail Hakki and Karag{\"o}z, Pinar},
  journal={Turkish Journal of Electrical Engineering and Computer Sciences},
  volume={30},
  number={4},
  pages={1404--1418},
  year={2022},
  doi={10.55730/1300-0632.3856}
}
```
