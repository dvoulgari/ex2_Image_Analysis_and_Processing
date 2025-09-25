# Chest X-Ray Image Analysis: Pneumonia Detection
This repository contains the Jupyter Notebook and necessary files for a machine learning assignment focused on classifying chest X-ray images to detect pneumonia.

## Project Objective

The main objective of this project is to develop and evaluate a deep learning model capable of accurately distinguishing between normal and pneumonia-affected chest X-ray images.

## Dataset

The analysis uses the Chest X-Ray Images (Pneumonia) dataset, available on Kaggle. It contains a large collection of X-ray images categorized as either NORMAL or PNEUMONIA.

Dataset URL: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

## Methodology

The notebook outlines a complete workflow for a deep learning classification task, covering the following key steps:

1) Data Loading and Initial Inspection: Loading the image data and performing an initial check to understand the distribution and characteristics of the images.

2) Preprocessing: Handling class imbalance, resizing images to a uniform dimension, and normalizing pixel values.

3) Model Architecture: Designing and training a Convolutional Neural Network (CNN) to learn features from the images.

4) Training & Evaluation: Training the model on the preprocessed dataset and evaluating its performance using metrics such as accuracy, precision, recall, and a confusion matrix.

## Repository Contents

- `notebook.ipynb`: The main Jupyter Notebook containing all the code, explanations, and results for the project.

- `requirements.txt`: A list of all Python libraries required to run the notebook.

## Getting Started

To view and run the notebook, follow these steps to set up your environment:

- Clone the Repository:

```bash
git clone https://github.com/dvoulgari/ex2_Image_Analysis_and_Processing.git
cd ex2_Image_Analysis_and_Processing
```
- Download the Dataset: Download the dataset from the Kaggle URL provided above and place the unzipped files in the project directory.

- Install Dependencies: Install the necessary Python packages listed in `requirements.txt`.

```bash
pip install -r requirements.txt
```

- Launch Jupyter Notebook: Open the `.ipynb` file to view and run the analysis.

```bash
jupyter notebook notebook.ipynb
```
