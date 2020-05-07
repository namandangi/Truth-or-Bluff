# Truth-or-Bluff
A supervised Machine Learning project

### Problem Statement 
A new employee is about to join a certain company,during his salary negotiation,the employee states that he was paid an annual salary of $160k.A guy from the HR department wants to determine whether the new recruit is telling the truth or bluffing.

### Introduction 
To determine the truth , the HR guy does some research and finds a list of 10 different position salaries of employees in the new recruit’s previous company.He also finds that the new recruit had been working as the Region Manager for 2 years and it takes approximately 4 years for an employee to be promoted to a higher position.

![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/dataset.png)

Since the new employee was half way from being promoted to the next level i.e, to level 7,therefore he was between level 6-7 (we will assume his level to be 6.5) before he left his previous company. On visualizing the data we realize,

![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/dataset_visualization.png)

there is a non-linear relationship between the position levels of the employees and their salaries in the new recruit’s previous company.

### Implementation 
On visualizing the data , we come to realize that we have a continuous labelled data set with a dependent factor (an employee salary, let’s say y) and an independent factor (an employee level ,let's say x) . Thus we can try implementing some supervised learning algorithms such as Polynomial regression,Decision Tree regression and lastly an Ensemble learning technique --Random Forest Regression.We can avoid techniques like linear regression because of non linear relationship and logistic regression because of the dataset is continuous in nature rather than discreet .

#####    Polynomial Regression
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/polyreg_1.png)
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/polyreg_2.png)

#####    Decision Tree Regression
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/decstree_1.png)
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/decstree_2.png)
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/decstree_3.png)

#####    Random Forest Regression
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/rf_1.png)
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/rf_2.png)
We try bumping up the number of trees in the random forest from 10 to 100
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/rf_3.png)
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/rf_4.png)
We try bumping up the number of trees in the random forest from 100 to 300
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/rf_5.png)
![](https://github.com/namandangi/Truth-or-Bluff/blob/master/public/rf_6.png)

### Conclusion 
Thus from the above implementations we can conclude that the employee is telling the truth as most of the implemented algorithms predicted salary values really close to the value which the employee stated.
