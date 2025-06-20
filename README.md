# Actuarial Loss Prediction – [Python]
[Python Code](https://github.com/YathharthhGarg/Actuarial_Loss_Prediction/blob/main/Actlpred.ipynb)

We were given 2 datasets as part of the project
[Training Dataset]( https://github.com/YathharthhGarg/Actuarial_Loss_Prediction/blob/main/train.csv) and [Testing Dataset]( https://github.com/YathharthhGarg/Actuarial_Loss_Prediction/blob/main/test.csv)

After finishing our Machine learning model, we came up with the ‘Ultimate claim cost incurred’ predictions as given in [Test+Prediction.xlsx]( https://github.com/YathharthhGarg/Actuarial_Loss_Prediction/blob/main/test%2Bprediction.xlsx)
---
## PART 1
In this part of our python code we cleaned both of our training and testing datasets in the following steps:
-	Removing Duplicates
-	Dealing with missing values
-	Fixing skewness of data which could impact our machine learning model
---

## PART 2
In this part of our python code we extracted data which was useful and removed the unnecessary columns.
-	Extracted Report delay days column which tells us the difference between date of injury and date of reporting the injury.
-	Extracted Hourly wages from weekly wages
-	Extracted just the number portion from the Claims number
-	Analysed the correlation matrix
---

## PART 3
In this part of our python code we performed a special type of string extraction. From the Column ‘Claim description’, we extracted the body part injured. In this way we can get a simple useful feature for our target rather than a column filled with text. 

---
## PART 4
In this part of our python code we either hot-one encoded or label encoded our categorical variables.
-	For simple features like Gender and Marital status, we used hot-one encoding
-	For complex features like Body parts we used Label encoding
-	Dropped any unnecassary columns/features

## PART 5
In this final part of our python code we first trained our model. Then by fitting the trained model on our testing set we got our predictions for ‘Ultimate Claim cost Incurred’ which was our target variable.


