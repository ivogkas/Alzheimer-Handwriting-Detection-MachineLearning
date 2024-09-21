# Alzheimer-Handwriting-Detection


## Overview
Team project for the Masters' degree course «Bio-Data Analysis» (2024). This project focuses on comparing various machine learning models to assess their effectiveness in diagnosing Alzheimer's disease through handwriting analysis. By leveraging data that captures the handwriting patterns of both patients with Alzheimer’s disease and healthy individuals, the goal is to identify the most suitable model for detecting this condition.

## Dataset Description

The [DARWIN dataset](https://archive.ics.uci.edu/dataset/732/darwin) was created to allow researchers to improve the existing machine learning methodologies for the prediction of Alzheimer's disease via handwriting analysis.. It includes detailed data from various handwriting tasks performed by individuals, providing a rich resource for developing and testing machine learning models.


### Dataset Details

- **Matrix Dimensions**: 174 rows x 452 columns
- **Participants**: 89 patients with Alzheimer’s disease, 85 healthy individuals
- **Tests**: 25 different handwriting tasks (Copying words and text, Drawing lines and shapes, Signature imitation etc.)
- **Features**: Each test comprises 18 numerical variables such as Writing speed, Total time taken, Pressure applied to the paper and more.
- **Labels**: Binary classification with labels:
  - “P” for patients with Alzheimer’s disease
  - “H” for healthy individuals


## Project Objectives and Methodology

The objective of this project was to develop the best possible machine learning model for predicting Alzheimer's disease based on handwriting analysis, and to understand the importance of each of the tasks in developing this model.

To achieve this, the methodology followed three main approaches:

1. **Full Dataset Analysis**: This approach involved analyzing the entire dataset to build the predictive model.
2. **Task-by-Task Analysis**: In this approach, each of the 25 tasks was analyzed individually to assess its contribution to the model's performance.
3. **Data Augmentation**: To enhance the robustness of our models and generate additional training data, we employed the Mixup technique. Mixup creates new training samples by combining pairs of examples with their corresponding labels, which helps in improving the generalization and performance of the models.
4. **Selective Task Analysis**: The most useful tasks, as identified in the task-by-task analysis, were used to build a model. The performance of this model was then compared with a model developed using the least useful tasks.
