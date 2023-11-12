# Wardrobe Wizard - Notebooks

This directory contains Jupyter notebooks for the Wardrobe Wizard project, focusing on Exploratory Data Analysis (EDA) and model training using Keras and TensorFlow.

## Structure

The notebooks are organized into two main subdirectories:

- `eda`: Contains notebooks for exploring and visualizing the data.
- `model_training`: Contains notebooks for training and experimenting with machine learning models.

## Notebooks Overview

### EDA

- `data_overview.ipynb`: Overview of the dataset, initial exploration of features, and data quality assessment.
- `data_visualization.ipynb`: Visualizations to understand the distributions, correlations, and patterns in the data.
- `data_preprocessing.ipynb`: Techniques for preprocessing the data to prepare it for modeling.

### Model Training

- `basic_cnn_model.ipynb`: Development and training of a basic Convolutional Neural Network (CNN) model.
- `advanced_cnn_model.ipynb`: Advanced modeling techniques, exploring different architectures and hyperparameters.
- `experiment_results.ipynb`: Analysis of model performance, comparison of different models, and final conclusions.

## Getting Started

To work with these notebooks, you should first ensure that your environment is correctly set up. This project uses `pipenv` for dependency management to ensure consistency across local and Docker environments.

### Local Setup

1. Navigate to the `notebooks` directory:

   ```bash
   cd notebooks
   ```
2. If you haven't already, initialize `pipenv` and install dependencies:

   ```bash
   pipenv --python 3.8
   pipenv install
   ```
3. Activate the `pipenv` environment and start Jupyter Notebook:

   ```bash
   pipenv shell
   jupyter notebook
   ```

### Using Docker

1. Build the Docker image (from the root of the `notebooks` directory):

   ```bash
   docker build -t wardrobe-wizard-notebooks .
   ```
2. Run the Docker container:

   ```bash
   docker run -p 8888:8888 wardrobe-wizard-notebooks
   ```
3. Access Jupyter Notebook at `http://localhost:8888` (or the URL provided in the terminal).

## Contribution

Feel free to contribute to these notebooks by adding new analyses, models, or improving existing ones. Ensure that any new dependencies are added to the `Pipfile` and documented accordingly.

---
