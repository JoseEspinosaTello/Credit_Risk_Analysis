# Credit_Risk_Analysis

# Overview

We have been taksed with determining the patterns of credit risk using a large credit card dataset from LendingClub. We will use several machine learning models to better understand trends withing the data. By creating oversampled, undersampled, and combination sampled machine learing models using different algorithms we hope to compare the results. If the models return similar results, we can assume the models can realiably predict loan risk.

### Resources

Technologies
-	Jupyter Notebook
-	Imbalanced-learn and sci-kit learn libraries for Pandas

## Results

## Naive Random Oversampling

![naive](https://github.com/JoseEspinosaTello/Credit_Risk_Analysis/blob/main/Resources/Images/naive.png)

Balanced Accuracy Score: 61.8%

Precision:

	- High-Risk: .01
	- Low-Risk: 1
	- Average: .99
Recall:

	- High-Risk: .63
	- Low-Risk: .61
	- Average: .61


## SMOTE Oversampling

![smoteOver](https://github.com/JoseEspinosaTello/Credit_Risk_Analysis/blob/main/Resources/Images/smoteOver.png)

Balanced Accuracy Score: 62%

Precision:

	- High-Risk: .01
	- Low-Risk: 1
	- Average: .99

Recall:

	- High-Risk: .59
	- Low-Risk: .65
	- Average: .65


## Undersampling

![undersampling](https://github.com/JoseEspinosaTello/Credit_Risk_Analysis/blob/main/Resources/Images/undersampling.png)

Balanced Accuracy Score: 53%

Precision:

	- High-Risk: .01
	- Low-Risk: 1
	- Average: .99

Recall:

	- High-Risk: .63
	- Low-Risk: .43
	- Average: .43

## Combination

![combination](https://github.com/JoseEspinosaTello/Credit_Risk_Analysis/blob/main/Resources/Images/combination.png)

Balanced Accuracy Score: 63.2%

Precision:

	- High-Risk: .01
	- Low-Risk: 1
	- Average: .99

Recall:

	- High-Risk: .68
	- Low-Risk: .58
	- Average: .58

## Ensemble Learner - Balanced Random Forest Classifier

![brfc](https://github.com/JoseEspinosaTello/Credit_Risk_Analysis/blob/main/Resources/Images/brfc.png)


Balanced Accuracy Score: 79%

Precision:

	- High-Risk: .03
	- Low-Risk: 1
	- Average: .99

Recall:

	- High-Risk: .68
	- Low-Risk: .90
	- Average: .90

## Ensemble Learner - AdaBoost

![ada](https://github.com/JoseEspinosaTello/Credit_Risk_Analysis/blob/main/Resources/Images/ada.png)


Balanced Accuracy Score: 93%

Precision:

	- High-Risk: .07
	- Low-Risk: 1
	- Average: .99

Recall:

	- High-Risk: .91
	- Low-Risk: .94
	- Average: .94

### Summary

By setting the random state of each model to 1, this allows us equally to compare the model results. Overall the ensemble models returned higher accuracy scores. The precision scores for all low risk scores were all 1, this meant the models all did well predicting the low risk scores. THe high risk precision scores varied meaning the models did not predict the high risk scores as accuratly. In the end the ensamble models were more accurate when it came to predicting the high/low risk scores and would be the better choice for the machine learning models.  