# Pipeline for Social Network Ads Classification

This repository contains a Python notebook (`using-pipeline.ipynb`) for building a machine learning pipeline to classify whether a person will purchase a product based on their information in a social network advertisement dataset.

## Dataset

The dataset used in this project is `Social_Network_Ads.csv`. It contains the following columns:

- `Age`: Age of the person
- `Gender`: Gender of the person
- `EstimatedSalary`: Estimated salary of the person
- `Purchased`: Whether the person purchased the product or not

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/abhiram-k-2223/ad-classifier-pipeline.git
    ```

2. Install the required Python packages:

    ```bash
    pip install pandas numpy scikit-learn
    ```

## Usage

1. Open and run the `using-pipeline.ipynb` notebook using Jupyter or any compatible notebook viewer.

2. The notebook will preprocess the data, build a machine learning pipeline using a Decision Tree Classifier, train the model, and evaluate its performance.

## Pipeline Steps

1. **Data Preprocessing**:
    - Drop the `User ID` column.
    - Split the data into training and testing sets.

2. **Feature Engineering**:
    - One-hot encode the `Gender` column.
    - Scale the `Age` and `EstimatedSalary` columns using StandardScaler.

3. **Model Training**:
    - Train a Decision Tree Classifier.

4. **Model Evaluation**:
    - Predict on the test set.
    - Calculate the accuracy score.

## Model Deployment

- The trained pipeline model is saved as `pipe.pkl` using pickle.

## Results

The model achieved an accuracy score of 83.75% on the test set.

## Other Approaches

- For an alternative approach to solving the same problem using Logistic Regression, check out [this repository](https://github.com/abhiram-k-2223/SocialAdsLogReg).
