# Deep Learning vs. Semi-Supervised Approaches: A Benchmark Study on Educational Data Mining for Student Performance Prediction

This repository contains the implementation of a **Deep Learning framwork** aimed at improving the semi-supervised feature selection approach presented by Yu et al. (2024). This enhanced methodology is designed to analyze and identify the most critical factors influencing student performance in educational datasets.

## Features

- **Deep Learning for Feature Selection**: Integrates DL techniques to refine the feature selection process.
- **Enhanced Semi-Supervised Learning**: Improves upon Yu et al.'s semi-supervised feature selection framework.
- **Extensive Evaluation Metrics**: Evaluates performance using accuracy, F1 score, precision, recall and ROC AUC.

## Dataset

The project uses the [xAPI Educational Dataset](https://www.kaggle.com/datasets/aljarah/xAPI-Edu-Data), which contains:

- 480 student records
- 16 features related to demographics, behavior, and academic performance
- Labels indicating performance levels: low, medium, and high

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/jalagrod/DL-ensemble-models-in-EDM.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Ensure you have Jupyter Notebook or an equivalent environment for running `.ipynb` files.

## Usage

1. **Run the Notebook**: Open and execute `DL.ipynb` in Jupyter Notebook.
2. **Deep Learning Model**: Utilize the provided DL-based feature selection model to rank feature importance.
3. **Classifier Evaluation**: Use the selected features to train classifiers and assess their performance.

## Key Files

- **`DL.ipynb`**: Notebook implementing the DL-based feature selection and evaluation.
- **`dataset_xapi.csv`**: Preprocessed dataset for feature selection and classification tasks.
- **`result.csv`**: Results of feature importance ranking and classifier evaluation.

## Methodology

This implementation introduces a DL-based feature selection method that enhances the semi-supervised approach by Yu et al. (2024):

1. **Data Preprocessing**:
   - Convert categorical data to numerical format.
   - Normalize feature values.

2. **Deep Learning Feature Selection**:
   - Train a neural network to learn feature weights.
   - Apply regularization to ensure interpretability of the selected features.

3. **Classifier Evaluation**:
   - Train classifiers using the selected features.
   - Evaluate using accuracy, precision, recall, and F1 score.

## Results

- The proposed DL-based method significantly improves the feature selection process, achieving higher accuracy and robustness compared to the semi-supervised method by Yu et al.
- Behavioral features such as **times of visiting resources** and **raising hands** remain critical predictors of student performance.

## Improvements Over Yu et al. (2024)

- **Predictive Capability**: The DL-based approach introduces predictive modeling, which was missing in the original semi-supervised feature selection framework.
- **Feature Interpretation**: Enhances interpretability and usability by learning explicit feature weights through the ANN.
- **Performance Gains**: Achieve improvements in classification accuracy.

## Future Work

- Extend the model to support larger and more complex educational datasets.

## Contact

For questions or collaboration opportunities:

- **Name**: Jose Antonio Lagares
- **Email**: jalargod@upo.es

