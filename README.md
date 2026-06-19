# Support Vector Machines (SVC, SVR, and LinearSVR)

This repository demonstrates the implementation of Support Vector Machine (SVM) algorithms using Scikit-Learn.

The project covers:

- Support Vector Classification (SVC)
- Support Vector Regression (SVR)
- Linear Support Vector Regression (LinearSVR)
- Kernel comparison
- Feature scaling
- Hyperparameter tuning using GridSearchCV
- Model evaluation


---

# Project 1 : Support Vector Classification (SVC)

## Objective

Build a multi-class classification model using the Iris dataset and evaluate the performance of different SVM kernels.

---

## Dataset

Dataset Used:

**Iris Dataset**

Loaded directly from Scikit-Learn.

Features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width


Target:

- Iris Setosa
- Iris Versicolor
- Iris Virginica


---

## Data Preprocessing

Performed the following preprocessing steps:

- Train-Test Split
- Feature Standardization using StandardScaler
- Stratified Sampling


---

## Models Implemented

### Default SVC (RBF Kernel)

```python
SVC()
```

### Linear Kernel

```python
SVC(kernel='linear')
```

### Polynomial Kernel

```python
SVC(kernel='poly')
```

### Sigmoid Kernel

```python
SVC(kernel='sigmoid')
```


### Hyperparameter Tuning

Different values of C were tested.

```python
C = [0.5,1,2,3,4,5]
```


---

## Evaluation Metrics

Models were evaluated using:

* Accuracy Score
* Classification Report
* Weighted F1 Score


---

# Project 2 : Support Vector Regression (SVR)

## Objective

Predict continuous target values using Support Vector Regression on the Diabetes dataset.


---

## Dataset

Dataset Used:

**Diabetes Dataset**

Loaded directly from Scikit-Learn.


Features:

10 Medical Variables


Target:

Disease Progression Measure


---

## Data Preprocessing


Performed:

* Train-Test Split
* Target Variable Scaling
* Standardization using StandardScaler


---

## Models Implemented


### Default SVR


```python
SVR()
```


### Linear Kernel


```python
SVR(kernel='linear')
```


### Polynomial Kernel


```python
SVR(kernel='poly')
```


### Sigmoid Kernel


```python
SVR(kernel='sigmoid')
```



---

## Hyperparameter Tuning


GridSearchCV was used to find optimal parameters.



Parameter Grid:


```python
param_grid = {

'C':[1,2,5,10,50,100],

'kernel':['rbf','linear'],

'epsilon':[0.01,0.1,0.2,0.3,0.5]

}
```


Cross Validation:

5-Fold Cross Validation


Scoring Metric:

R² Score


---

## Best Model

Example:


```python
SVR(kernel='linear',
    C=10,
    epsilon=0.1)
```


---

# Project 3 : LinearSVR


LinearSVR was implemented as an efficient alternative to SVR with a linear kernel.



Example:


```python
LinearSVR(

C=10,

epsilon=0.1,

max_iter=5000

)
```


---

## Evaluation Metrics


Regression models were evaluated using:


* R² Score


Metrics calculated:


* Training R²
* Testing R²


---

# Libraries Used


```python
pandas
numpy
scikit-learn
```



---

# Project Structure


```text
├── svc_implementation.ipynb
├── svr_implementation.ipynb
├── README.md
```


---

# Key Concepts Covered


✔ Support Vector Classification

✔ Support Vector Regression

✔ LinearSVR

✔ Kernel Functions

✔ Feature Scaling

✔ Standardization

✔ Hyperparameter Tuning

✔ GridSearchCV

✔ Cross Validation

✔ Model Evaluation

✔ Classification Metrics

✔ Regression Metrics


---

## Author

Shanu
