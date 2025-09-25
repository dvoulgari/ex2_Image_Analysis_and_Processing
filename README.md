# Chest X-Ray Image Analysis: Pneumonia Detection
This repository contains the Jupyter Notebook and necessary files for a machine learning assignment focused on classifying chest X-ray images to detect pneumonia.

## Project Objective

The main objective of this project is to develop and evaluate a deep learning model capable of accurately distinguishing between normal and pneumonia-affected chest X-ray images.

## Dataset

The analysis uses the Chest X-Ray Images (Pneumonia) dataset, available on Kaggle. It contains a large collection of X-ray images categorized as either NORMAL or PNEUMONIA.

Dataset URL: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

## Methodology

The notebook outlines a complete workflow for a deep learning classification task, covering the following key steps:

Chest X-Ray Image Analysis: Pneumonia Detection
This repository contains the Jupyter Notebook and necessary files for a machine learning assignment focused on classifying chest X-ray images to detect pneumonia.

Project Objective

The main objective of this project is to develop and evaluate a deep learning model capable of accurately distinguishing between normal and pneumonia-affected chest X-ray images.

Dataset

The analysis uses the Chest X-Ray Images (Pneumonia) dataset, available on Kaggle. It contains a large collection of X-ray images categorized as either NORMAL or PNEUMONIA.

Dataset URL: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

## Methodology

The notebook outlines a complete workflow for a deep learning classification task, covering the following key steps:

1) Data Loading and Initial Inspection: Loading the image data and performing an initial check to understand the distribution and characteristics of the images.

2) Preprocessing: The notebook addresses the challenge of a highly imbalanced dataset and explains the preprocessing choices, including resizing images and normalizing pixel values. It also mentions a better data splitting strategy using stratify to ensure the same imbalance ratio across all splits.

3) Model Architecture: The project compares three different models: a custom Convolutional Neural Network (CNN), a pre-trained VGG16 model, and a classical machine learning model (Random Forest).

4) Training & Evaluation: Each model is trained and its performance is evaluated using a variety of metrics, including accuracy, precision, recall, and a confusion matrix.

---

### Model Comparison and Results

The project's key findings are based on a comparison of the three models' performance.

- Custom CNN: Achieved the highest overall performance, particularly in recall (0.993) and ROC AUC (0.998). This indicates its strong ability to identify true pneumonia cases with very few false negatives.

- VGG16: This model demonstrated the highest precision (0.992), suggesting it rarely misclassifies a normal case as pneumonia. However, its slightly lower recall (0.948) indicates it may miss more true pneumonia cases compared to the other models.

- Random Forest: Performed robustly across all metrics with a strong balance between precision and recall, and its ROC AUC of 0.99 nearly matched the custom CNN, making it a competitive alternative to deep learning models.

In conclusion, while all models performed strongly, the Custom CNN provides the best balance between sensitivity and specificity and would be the most reliable for deployment in clinical screening contexts.

<table>
  <tr>
    <td style="text-align: center;">
      <img src="https://github.com/dvoulgari/ex2_Image_Analysis_and_Processing/blob/main/notebook/models_comp.png" alt="Models' comparison with 95% intervals" width="450">
      <br>
      *Figure 1: Models' comparison with 95% intervals*
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/dvoulgari/ex2_Image_Analysis_and_Processing/blob/main/notebook/ROC_curves.png" alt="ROC curves of the plots" width="450">
      <br>
      *Figure 2: ROC curves of the plots*
    </td>
  </tr>
</table>

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
