# Parameter Optimization of SVM
Assignment for UCS654

## Written By
Name : Sehajbir Singh Mann
  
Roll No. : 102003478

Sub-Group: 3CO19

## About SVM and Parameter Optimization

Support Vector Machine or SVM is one of the most popular Supervised Learning algorithms, which is used for Classification as well as Regression problems. However, primarily, it is used for Classification problems in Machine Learning.

Some of the most important parameters of SVM such as kernel, C, and gamma can be changed in order to achieve a higher accuracy. This is called as Hyperparameter Tuning. 

We can perform this task using GridSearchCV for optimizing these parameters.

In this python file, I've used a Fitness Function to optimize the parameters.

## Dataset

The dataset for the project has been downloaded from the UCI Machine Learning Repository.
[https://archive.ics.uci.edu/ml/datasets/Room+Occupancy+Estimation](https://archive.ics.uci.edu/ml/datasets/Room+Occupancy+Estimation)

This dataset is used for estimating the precise number of occupants in a room using multiple non-intrusive environmental sensors like temperature, light, sound, CO2 and PIR. It is a multi-variate classification Dataset.

Number of Instances: 10129

Number of Attributes: 16

## Final Result Table

| Sample  | Best Accuracy | Best Kernel | Best Nu | Best Epsilon |
| -----   | ------------- | ----------- | ------- | ------------ |
| 1 | 0.83 | RBF | 9.46 | 9.25 |
| 2 | 0.96 | Poly | 6.65 | 1.49 |
| 3 | 0.96 | Poly | 3.83 | 1.30 |
| 4 | 0.96 | RBF | 2.78 | 0.20 |
| 5 | 0.89 | Poly | 3.69 | 2.33 |
| 6 | 0.84 | Poly | 8.91 | 2.17 |
| 7 | 0.94 | Poly | 5.06 | 9.38 |
| 8 | 0.96 | Linear | 1.91 | 8.23 |
| 9 | 0.96 | Poly | 3.48 | 1.91 |
| 10 | 0.90 | Poly | 2.22 | 9.79 |

## Convergence Graph
![graph](https://user-images.githubusercontent.com/72306997/233000047-3bbc6cf2-8ec0-4276-8519-17da7da2fb25.png)

## Discussion
From the above graph, we can conclude that the model is well trained and parameter have been optimized due to the less gap between training and cross-validation curve.

The graph is made for the sample which has best accuracy. Sample 2 has the best accuracy of 0.96 having kernel = Poly, Nu = 6.65 and Epsilon = 1.49.
