# Rice Leaf Disease Detection Using Deep Learning

## Project Overview

Rice Leaf Disease Detection is a Deep Learning project that uses Convolutional Neural Networks (CNN) to classify rice leaf images into different disease categories.

The main objective is to analyse rice leaf images and identify diseases automatically using image classification techniques.

## Problem Statement

Rice plants are affected by different diseases that can reduce crop quality and agricultural productivity. Identifying these diseases at an early stage can help farmers take appropriate action.

This project develops a CNN-based image classification system to identify three rice leaf disease categories.

## Dataset

The dataset contains rice leaf images belonging to three classes:

1. Bacterial Leaf Blight
2. Brown Spot
3. Leaf Smut

| Disease Class | Number of Images |
|---|---:|
| Bacterial Leaf Blight | 40 |
| Brown Spot | 40 |
| Leaf Smut | 39 |
| **Total** | **119** |

**Note:** The assignment document mentions 120 images, but the available dataset contains 119 images.

## Technologies Used

- Python
- Jupyter Notebook
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- PIL (Pillow)

## Project Workflow

1. Dataset Loading and Extraction
2. Exploratory Data Analysis (EDA)
3. Image Preprocessing
4. Image Resizing
5. Image Normalization
6. Label Encoding
7. Train-Test Splitting
8. Data Augmentation
9. CNN Model Development
10. Model Training and Evaluation
11. Model Comparison
12. Final Conclusion

## Data Augmentation Techniques

The following techniques were applied to increase variations in the training images:

- Rotation
- Horizontal Flipping
- Zoom
- Contrast Adjustment

The training dataset was expanded from 95 original images to 475 image variations. The test dataset was kept unchanged.

## CNN Model Development

Two CNN architectures were developed and evaluated.

### Model 1

- Training Accuracy: 87.16%
- Testing Accuracy: 70.83%
- Testing Loss: 0.5176

### Model 2

- Training Accuracy: 100%
- Testing Accuracy: 54.17%
- Testing Loss: 1.3587

## Model Comparison

Model 1 performed better than Model 2 on the test dataset.

Model 2 achieved 100% training accuracy but lower testing accuracy, indicating overfitting.

Based on the current experimental results, Model 1 is the better-performing model among the two tested architectures.

Further testing with a larger and independent dataset is required before production deployment.

## Challenges Faced

- The available dataset contained 119 images instead of the 120 mentioned in the assignment.
- Images had different dimensions.
- A small dataset created a risk of model overfitting.
- Data augmentation was required to increase training image variations.
- GPU support was unavailable in the native Windows environment, so training was performed using the CPU.

## Project Structure

```text
Rice-Leaf-Disease-Detection/
│
├── Rice_Leaf_Disease_Detection.ipynb
├── README.md
│
├── Bacterial leaf blight/
├── Brown spot/
└── Leaf smut/
```

The dataset folders contain the images used for training and testing.

## How to Run the Project

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Folder

```bash
cd Rice-Leaf-Disease-Detection
```

### 3. Install Required Libraries

```bash
pip install numpy pandas matplotlib seaborn tensorflow pillow
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the Notebook

Open `Rice_Leaf_Disease_Detection.ipynb` and execute all cells from beginning to end.

Ensure that the dataset ZIP files or extracted dataset folders are available in the expected working directory.

## Conclusion

This project demonstrates how Deep Learning and Convolutional Neural Networks can be used for rice leaf disease classification.

Two CNN models were developed and compared. Model 1 achieved 70.83% testing accuracy and performed better than Model 2.

The project provides practical experience in image preprocessing, data augmentation, CNN model development, and model evaluation.

## Author

**K. Pranay**

B.Tech – Computer Science and Engineering (Artificial Intelligence and Machine Learning)

## Project Type

Data Science / Deep Learning / Image Classification
