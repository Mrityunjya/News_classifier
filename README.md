# News Classification with Python and Scikit-Learn

## Overview

This project demonstrates how to build a news classification model using Python and `scikit-learn`. The model is trained on the 20 Newsgroups dataset and can classify news articles into various categories. The project also includes visualization of the model's performance and data distribution.

## Features

- **Text Classification**: Classifies news articles into 20 predefined categories.
- **Model Evaluation**: Provides accuracy, classification report, and confusion matrix.
- **Visualization**: Includes plots for confusion matrix, top features by log-probability, and document length distribution.

## Prerequisites

Make sure you have the following software installed:

- Python 3.6 or higher
- `pip` for installing Python packages

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/news-classification.git
   cd news-classification
   ```

2. **Install Required Packages**

   Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

   Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. **Requirements File**

   Create a file named `requirements.txt` with the following content:

   ```
   numpy
   pandas
   matplotlib
   seaborn
   scikit-learn
   ```

## Usage

1. **Run the Script**

   Execute the Python script to train the model, evaluate it, and generate visualizations:

   ```bash
   python news_classification.py
   ```

2. **Review Results**

   The script will output the accuracy, classification report, and display several plots:
   - **Confusion Matrix**: Shows the performance of the classifier.
   - **Top 10 Features**: Displays the most influential features (words) for classification.
   - **Document Length Distribution**: Visualizes the distribution of document lengths.

## Code Explanation

### `news_classification.py`

- **Data Loading**: Loads the 20 Newsgroups dataset using `fetch_20newsgroups`.
- **Preprocessing**: Converts text data into numerical features using `TfidfVectorizer`.
- **Model Training**: Trains a `MultinomialNB` classifier on the TF-IDF features.
- **Evaluation**: Computes accuracy, generates a classification report, and creates a confusion matrix.
- **Visualization**: Plots the confusion matrix, top features, and document length distribution.

## Testing

1. **Run the Script**: Make sure all required packages are installed and run `news_classification.py` to test the model.
2. **Check Output**: Review the printed accuracy and classification report, and analyze the generated plots.

## Troubleshooting

- **Missing Packages**: Ensure all packages in `requirements.txt` are installed. Run `pip install -r requirements.txt` if needed.
- **Plot Issues**: If plots do not display, check your Python environment and ensure you have a GUI backend for `matplotlib`.
