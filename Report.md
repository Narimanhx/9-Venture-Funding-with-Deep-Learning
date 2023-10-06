# Module13Challenge
# Neural Network for Applicant Success Prediction
![Venture Funding](Images/13-challenge-image.png)

## Overview
This project aims to build and optimize a neural network to predict the success of applicants based on various features. The dataset, `applicants_data.csv`, contains information related to applicants, and the goal is to create a binary classification model to determine whether an applicant will be successful.

## Project Structure

### 1. Data Preparation:
   * **Loading Data:** Imported the dataset into a Pandas DataFrame.
   * **Data Cleaning:** Removed unnecessary columns and handled missing values.
   * **Encoding Categorical Variables:** Applied OneHotEncoder to encode categorical variables.
   * **Splitting Data:** Created feature (`X`) and target (`y`) datasets and split them into training and testing sets.
   * **Scaling:** Standardized the features using StandardScaler.

### 2. Neural Network Models:
   * **Base Model:** Created a two-layer deep neural network model with the `relu` activation function.
   * **Alternative Models:** Developed three additional models with variations in architecture to optimize performance.
   * **Training & Evaluation:** Compiled and trained models using `binary_crossentropy` loss, `adam` optimizer, and the `accuracy` evaluation metric. Evaluated models on test data to obtain loss and accuracy.

### 3. Optimization:
   * Adjusted input data, neurons, hidden layers, activation functions, and epochs to optimize accuracy.
   * Created and evaluated alternative models.

### 4. Model Saving:
   * Saved the best-performing model and alternative models to HDF5 files.

## Results
### Original Model:
* Loss: 0.55059
* Accuracy: 0.73072

### Alternative Model 1:
* Loss: 0.55802
* Accuracy: 0.72827

### Alternative Model 2:
* Loss: 0.55245
* Accuracy: 0.72956

## Conclusion and Recommendation
The project successfully built and evaluated neural network models for predicting applicant success. While all models demonstrated reasonably good accuracy, the Original Model outperformed the alternative models with the highest accuracy of approximately 73.1%. However, its loss was relatively high, indicating a potential challenge in generalization.

It is recommended to further explore optimization strategies, including hyperparameter tuning and potentially different model architectures, to improve accuracy and reduce loss. Additionally, the project should consider collecting more data or enhancing feature engineering to potentially enhance model performance further.