# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.


2.Import the dataset to operate on.


3.Split the dataset.


4.Predict the required output.


5.End the program.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: DIVAKAR R
RegisterNumber: 212222240026

import chardet
file='/content/spam.csv'
with open(file,'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result


import pandas as pd
data=pd.read_csv('/content/spam.csv',encoding='Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values
y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

*/
```

## Output:



Result output



![ml901](https://github.com/divakar618/Implementation-of-SVM-For-Spam-Mail-Detection/assets/121932143/f204779c-ddb5-4ae2-993f-ae341b3c57ef)


data.head()



![ml902](https://github.com/divakar618/Implementation-of-SVM-For-Spam-Mail-Detection/assets/121932143/bb0e991a-9152-405f-9e5e-c2c4825aeaa3)



data.info()



![ml903](https://github.com/divakar618/Implementation-of-SVM-For-Spam-Mail-Detection/assets/121932143/ca536842-83c6-42fb-92c8-39857d6a2263)



data.isnull().sum()



![ml904](https://github.com/divakar618/Implementation-of-SVM-For-Spam-Mail-Detection/assets/121932143/39d7cb7d-7412-4573-9feb-f6ac1efb04f3)



Y_prediction 


![ml905](https://github.com/divakar618/Implementation-of-SVM-For-Spam-Mail-Detection/assets/121932143/ff930369-fb5c-48d6-958f-89eb0045fdf0)



Accuracy value



![ml906](https://github.com/divakar618/Implementation-of-SVM-For-Spam-Mail-Detection/assets/121932143/d7716f71-9d06-4856-a9b1-887e937ce0a9)







## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
