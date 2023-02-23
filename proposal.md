# Project Proposal Group044

## Names
* Ryan Kabbes  
* Jiaohaer Taolan  
* Gyujin Hong  
* Tej Nair

## Abstract
The goal of the project is to compare different machine learning models for predicting whether a person's income is above or below $50K using the UCI Adult dataset based on a set of demographic and socioeconomic features including workclass, education level, marital-status, occupation, relationship, race, sex, and native country. The data needs to be processed and cleaned by converting categorical variables into numerical ones and performing feature scaling. The missing values will also need to be filled in. The models that are being tested include but are not limited to: Logistic Regression, K-Nearest Neighbors, and Decision Tree. The aim is to find the best-performing model that could accurately predict a person's income level and to evaluate the performance of different models based on their accuracy,recall, precision, F-measure and ROC Curve.


## Background  
There has been a significant amount of prior work using the Adult dataset for various machine learning and data analysis tasks. One common application of the dataset is predicting income levels based on demographic and financial information.

For instance, a study by Lu et al. (2017) used the Adult dataset to compare the performance of various machine learning algorithms for predicting income levels. The authors found that random forests and gradient boosting were among the most accurate algorithms for this task.

Another study by Chen et al. (2017) used the Adult dataset to explore the impact of education and occupation on income levels. The authors found that higher levels of education and certain occupations (such as managerial positions) were associated with higher incomes.

In addition, there has been work on exploring the fairness and bias implications of using the Adult dataset for machine learning tasks. For example, a study by Feldman et al. (2015) investigated the fairness of predicting income levels based on the Adult dataset, finding that certain demographic groups (such as women and African Americans) were more likely to be misclassified by the predictive model.  

Overall, the Adult dataset has been widely used in various machine learning and data analysis applications, with prior work focusing on tasks such as predicting income levels, exploring the impact of demographic and financial factors on income, and investigating fairness and bias issues.  

The dataset has been widely used in research for tasks such as predicting income levels and understanding the factors that influence income. However, it's important to note that the dataset has some limitations, such as being based on data from 1994 and not including information on factors such as race or ethnicity. Nonetheless, the Adult dataset remains a valuable resource for exploring various topics in machine learning and data analysis. 

## Problem Statement  
The problem that we are solving is to predict whether an individual's annual income is above or below $50K based on a set of demographic and socioeconomic features. The task is a binary classification problem where the output variable can only take two possible values: 1 (income greater than $50K) or 0 (income less than or equal to $50K).

The dataset used for this task is the UCI Adult dataset, which contains 14 features such as age, workclass, education level, marital status, occupation, relationship, race, sex, and native country. These features are used as inputs to the machine learning models to predict the target variable, which is the income level.  

The problem can be expressed mathematically as follows:

Given a set of N individuals represented as `(x_1, y_1), (x_2, y_2), ..., (x_N, y_N)`, where `x_i` represents the values of the 14 input features for the ith individual and `y_i` is the binary target variable indicating whether the ith individual's income is greater than $50K or not, the goal is to learn a function `f(x)` that can accurately predict `y` for new individuals based on their input features.

In other words, the problem is to find a function `f(x)` such that `y_i ≈ f(x_i)` for all `i = 1, 2, ..., N`, where `≈` denotes approximate equality. The function `f(x)` is learned from a training set of labeled data (x_i, y_i) using different machine learning models and evaluated on a test set of labeled data to determine its predictive accuracy.   


## Data 

The data we will use in our final project is the dataset called "Adult" from the UCI Machine Learning Repository. The data includes demographic and financial information for over 32,000 individuals in the United States. The dataset was extracted from the 1994 United States Census Bureau data and was split into train-test using MLC++ GenCVFiles (2/3, 1/3 random). The data has 48842 instances in total, which is the mix of continuous and discrete    (train=32561, test=16281). There would be 45222  instances left if instances with unknown values are removed (train=30162, test=15060).

The dataset includes 14 attributes, such as age, workclass, education level, marital status, occupation, and hours worked per week.  
The dataset contains a mix of categorical and numeric type data.  
Categorical Attributes include:  
* workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.     
Individual work category  
* education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.  
Individual’s highest education degree  
* marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.    
    Individual marital status  
* occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspect, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.  
Individual’s occupation  
* relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.  
Individual’s relation in a family  
* race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.  
Race of Individual  
* sex: Female, Male.  
* native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinidad Tobago, Peru, Hong, Holland-Netherlands.  
Individual’s native country  
And the continuous attributes include:  
* age: continuous.  
Age of an individual  
* fnlwgt: final weight, continuous.  
* The weights on the CPS files are controlled to independent estimates of the civilian noninstitutional population of the US. These are prepared monthly for us by Population Division here at the Census Bureau.  
* capital-gain: continuous.  
* capital-loss: continuous.  
* hours-per-week: continuous.  
Individual’s working hour per week


The link to obtain the data can be found [here](https://archive.ics.uci.edu/ml/datasets/Adult).  
  
## Proposed Solution   

We will use different classification algorithms, include:   
* Logistic Regression  
* K-Neareat Neighbor  
* Decision Trees   

And if we had more time we will explore:  
* Artificial Neural Network   
* Support Vector Machine   

and so on.  And the benchmark model would be the Logistic Regression.  
The python packages will include:  
* Scikit-learn  
* Pandas  
* Numpy  
* Matplotlib  



## Evaluation Matrix
  
We will use different eveluation matrix to compare the different model performance.First, we would like to use overall performance statistics which includes accuracy, recall, precision, F1 measure and so on to have a overall sensation of the models. Then we will be using more complex model evaluator AUC-ROC.

## Ethics & Privacy
This project deals with personal data may have ethical and privacy implications. The data used in the project includes sensitive information such as race, gender, there could be concerns about potential discrimination or bias in the models developed. The data was obtained by UCI and they did not violate any privacy issues or acquire the data without proper consent/authorization. To address these issues. There are missing values in the data and therefore there may be some bias in the data itself. We plan to evaluate all the variables and their relation to the answer of the question. The data itself is a public dataset and if the data becomes no longer public or needs to be removed, then it will be eliminated. The data will be analyzed thoroughly and we will make visuals to represent the entirety of the data to avoid bias. We strive to use the data for its intended use of predicting whether a person’s income is above or below $50k and to use a multitude of models to evaluate the best model.  


## Team Expectations
* 	We plan on meeting at least once a week in order to establish roles and evaluate progress.
* 	We expect to work asynchronously throughout the week on the project.
* 	We expect each group member to put in equivalent work.
* 	We expect that each group member is active and responsibly handles their workload.
* 	We expect that group members do not take more than 1 day to respond to queries.
* 	We will handle conflict and difficulty with fairness.
* 	We expect positive interactions and efficient teamwork.
* 	So far only two out of four group members have contributed/made contact.
 

## Project Timeline Proposal  

| Time          |  Content|  Specification|
|---------------|---------|---------------|
| 2/20/23 8 PM | Brainstorm topics/questions | Determine best form of communication; Discuss and decide on final project topic; discuss hypothesis; begin background research| 2/21/23  8 PM |Find dataset after deciding on topic	|Decide topic and look for data sets. |
2/22/23	8 PM|	Edit, finalize, and submit proposal|	Discuss possible models and assign tasks to group.  |
2/27/23	8 PM	|Clean Data and begin Analysis	|Filter through dataset and allow for analysis to begin.  
3/1/23	8 PM	|Continue Analysis	|Discuss/edit project code and problem solve if need be.  |
3/8/23	8 PM	|NA|	Turn in check point  |
3/15/23	8 PM	|Complete Analysis and begin project Conclusion	|Discuss/edit full project  |
3/19/23	8 PM	|Review project and prepare for completion	|Overview of project. Project should be nearly finished.  |
3/22/22	8 PM	|NA|	Turn in Final Project|
      


##   References:  
 
* Chen, X., Wang, Y., & Xue, M. (2017). The Impact of Education and Occupation on Income Levels: A Case Study of the United States. Journal of Economics, Business and Management, 5(7), 241-245.  
* Feldman, M., Friedler, S. A., Moeller, J., Scheidegger, C., & Venkatasubramanian, S. (2015). Certifying and removing disparate impact. ACM SIGKDD Conference on Knowledge Discovery and Data Mining, 259-268.  
* Lu, Y., Poirson, P., Ricketts, T., & Sun, Y. (2017). Comparison of machine learning algorithms for predicting income levels. Journal of Big Data, 4(1), 1-11.