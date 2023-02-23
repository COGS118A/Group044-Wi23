# Project Proposal
## The adult data

## Abstract
The goal of the project is to compare different machine learning models for predicting whether a person's income is above or below $50K using the UCI Adult dataset based on a set of demographic and socioeconomic features including workclass, education level, marital-status, occupation, relationship, race, sex, and native country. The data needs to be processed and cleaned by converting categorical variables into numerical ones and performing feature scaling. The missing values will also need to be filled in. The models that are being tested include but are not limited to: Logistic Regression, K-Nearest Neighbors, and Decision Tree. The aim is to find the best-performing model that could accurately predict a person's income level and to evaluate the performance of different models based on their accuracy, precision, and F-measure.


## Background  
There has been a significant amount of prior work using the Adult dataset for various machine learning and data analysis tasks. One common application of the dataset is predicting income levels based on demographic and financial information.

For instance, a study by Lu et al. (2017) used the Adult dataset to compare the performance of various machine learning algorithms for predicting income levels. The authors found that random forests and gradient boosting were among the most accurate algorithms for this task.

Another study by Chen et al. (2017) used the Adult dataset to explore the impact of education and occupation on income levels. The authors found that higher levels of education and certain occupations (such as managerial positions) were associated with higher incomes.

In addition, there has been work on exploring the fairness and bias implications of using the Adult dataset for machine learning tasks. For example, a study by Feldman et al. (2015) investigated the fairness of predicting income levels based on the Adult dataset, finding that certain demographic groups (such as women and African Americans) were more likely to be misclassified by the predictive model.  

Overall, the Adult dataset has been widely used in various machine learning and data analysis applications, with prior work focusing on tasks such as predicting income levels, exploring the impact of demographic and financial factors on income, and investigating fairness and bias issues.

## Problem Statement
Clearly describe the problem that you are solving. The problem should be well defined. Additionally, describe the problem throughly such that it is clear that the problem is quantifiable problem and can be expressed in mathmatical or logical terms.  

The target variable is a binary classification indicating whether an individual's annual income is greater than $50,000 or not.  


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







The dataset has been widely used in research for tasks such as predicting income levels and understanding the factors that influence income. However, it's important to note that the dataset has some limitations, such as being based on data from 1994 and not including information on factors such as race or ethnicity. Nonetheless, the Adult dataset remains a valuable resource for exploring various topics in machine learning and data analysis. 

The link to obtain the data can be found [here](https://archive.ics.uci.edu/ml/datasets/Adult).  
  
## Proposed Solution
In this section, clearly describe a solution to the problem. The solution should be applicable to the project domain and appropriate for the dataset(s) or input(s) given. Provide enough detail (e.g., algorithmic description and/or theoretical properties) to convince us that your solution is applicable. Why might your solution work? Make sure to describe how the solution will be tested.

If you know details already, describe how (e.g., library used, function calls) you plan to implement the solution in a way that is reproducible.

If it is appropriate to the problem statement, describe a benchmark model[3] against which your solution will be compared.  

## Evaluation Matrix
Propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms).  


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

2/20/23	8 PM	Brainstorm topics/questions	Determine best form of communication; Discuss and decide on final project topic; discuss hypothesis; begin background research  

2/21/23	8 PM	Find dataset after deciding on topic	Decide topic and look for data sets.  

2/22/23	8 PM	Edit, finalize, and submit proposal	Discuss possible models and assign tasks to group.  

2/27/23	8 PM	Clean Data and begin Analysis	Filter through dataset and allow for analysis to begin.  

3/1/23	8 PM	Continue Analysis	Discuss/edit project code and problem solve if need be.  

3/8/23	8 PM	NA	Turn in check point  

3/15/23	8 PM	Complete Analysis and begin project Conclusion	Discuss/edit full project  

3/19/23	8 PM	Review project and prepare for completion	Overview of project. Project should be nearly finished.  

3/22/22	8 PM	NA	Turn in Final Project


## Footnotes    

[^Chen, X., Wang, Y., & Xue, M. (2017). The Impact of Education and Occupation on Income Levels: A Case Study of the United States. Journal of Economics, Business and Management, 5(7), 241-245.]  
[^要注明的文本]  
