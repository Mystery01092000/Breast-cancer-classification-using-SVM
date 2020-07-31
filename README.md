# Breast Cancer Classification using Support Vector Machine

![We fight](https://www.legacycommunityhealth.org/wp-content/uploads/2018/10/breast-cancer-pink-ribbon-1.png)

## ======Together We Fight Breast Cancer=====

# Understanding:
Breast cancer is cancer that forms in the cells of the breasts.

After skin cancer, breast cancer is the most common cancer diagnosed in women. Breast cancer can occur in both men and women, but it's far more common in women.

![biopic](https://www.mayoclinic.org/-/media/kcms/gbs/patient-consumer/images/2013/11/15/17/39/ds00328_-ds00982_-ds000983_-ds01063_-ds01070_-hq00348_im01880_r7_breastthu_jpg.png)

Substantial support for breast cancer awareness and research funding has helped created advances in the diagnosis and treatment of breast cancer. Breast cancer survival rates have increased, and the number of deaths associated with this disease is steadily declining, largely due to factors such as earlier detection, a new personalized approach to treatment and a better understanding of the disease.
Early diagnosis significantly increases the chances of surviver. The key challenges against it's detection is how to classify tumors into malignant(Cancer) or benign(not cancer). A tumor is considered malignant (Cancer) if the cells can grow into surrounding tissues or spread to distant areas of the body. A benign tumor does not invade nearby tissue or spread to other parts of the body the way cancer can. But benign tumors can be serious if they press on vital structures such as blood vessel or nerves.

### For more: [Breast Cancer](https://www.cancer.org/cancer/breast-cancer/about/what-is-breast-cancer.html)

### Why Machine Learning for classification?
* Machine Learning technique can dramatically improve the level of diagnosis in breast cancer. Research shows that experience physicians can detect cancer by 79% accuracy, while 91%(up to 97%) accuracy can be achieved using Machine Learning techniques.

## Project Task:
In this project, our study is concerned with the tumors as are malignant (i.e., Cancerous) and benign (i.e., Non Cancerous) using features obtained from several cell images.


# Dataset:
  Dataset is taken from sklearn datasets and can be imported using "from sklearn.datasets import load_breast_cancer"
  Link for the dataset: [Breast_cancer_dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)

## Features (Columns) Description:
  ![Imp](https://miro.medium.com/max/1400/1*jxDWsQAM6-6e4IAk-CDsAg.png)

  
# Model Used and Modeling

# ***Support Vector Machines (SVM)*** -

## What is Support Vector Machine ?

A Support Vector Machine (SVM) is a binary linear classification whose decision boundary is explicitly constructed to minimize generalization error. It is a very powerful and versatile Machine Learning model, capable of performing linear or nonlinear classification, regression and even outlier detection.

SVM is well suited for classification of complex but small or medium sized datasets.

## How does SVM classify?

It’s important to start with the intuition for SVM with the special linearly separable classification case.
If classification of observations is “linearly separable”, SVM fits the “decision boundary” that is defined by the largest margin between the closest points for each class. This is commonly called the “maximum margin hyperplane (MMH)”.

![svm](https://miro.medium.com/max/2000/1*glixBGaKMiVDhWFwkA3yoQ.png)

### The advantages of support vector machines are:
* Effective in high dimensional spaces.
* Still effective in cases where number of dimensions is greater than the number of samples.
* Uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.
* Versatile: different Kernel functions can be specified for the decision function. Common kernels are provided, but it is also possible to specify custom kernels.


### The disadvantages of support vector machines include:
* If the number of features is much greater than the number of samples, avoid over-fitting in choosing Kernel functions and regularization term is crucial.
* SVMs do not directly provide probability estimates, these are calculated using an expensive five-fold cross-validation (see Scores and probabilities).


## After, SVM we use SVM on Normalized data

## Gridsearch Model :
  Improved our model by searching the best hyperparameter using GridSearch.
  
  
# Result:
 ### Model : SVM with normalized data and SVM with best hyperparameter (i.e., Grid Search) performed Equally well.
 ### Accuracy : 96 % 
 ### Successful in training our model using SVM-SVC, with an excellent result.
 
 
 
 
## Sources :
1. https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html
2. https://en.wikipedia.org/wiki/Support_vector_machine
3. https://towardsdatascience.com/breast-cancer-classification-using-support-vector-machine-svm-a510907d4878
4. https://www.geeksforgeeks.org/svm-hyperparameter-tuning-using-gridsearchcv-ml/
