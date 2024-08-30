# Alzheimer-Handwriting-Detection


## Overview
Team project for the Masters' degree course «Bio-Data Analysis» (2024). This project focuses on comparing various machine learning models to assess their effectiveness in diagnosing Alzheimer's disease through handwriting analysis. By leveraging data that captures the handwriting patterns of both patients with Alzheimer’s disease and healthy individuals, the goal is to identify the most suitable model for detecting this condition. The primary aim of this endeavor is to enhance the early and accurate diagnosis of Alzheimer’s disease using a non-invasive method, thereby contributing to a better understanding and management of the disease.

## Dataset Description

The dataset used in this project is the largest available dataset for analyzing handwriting patterns in the context of Alzheimer's disease, as reported by Clica et al. (2022). It consists of a matrix with dimensions 174 x 452 and includes data from 89 patients diagnosed with Alzheimer’s disease and 85 healthy individuals.

### Dataset Details

- **Matrix Dimensions**: 174 rows x 452 columns
- **Subjects**: 89 patients with Alzheimer’s disease, 85 healthy individuals
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
