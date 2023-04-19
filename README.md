# Tuberculosis X-Ray Image Classification

This project aims to classify chest x-ray images as either normal or indicating tuberculosis using deep learning techniques. Tuberculosis is a bacterial infection that most commonly affects the lungs. People with tuberculosis in their lungs can spread the bacteria when they cough, sneeze, or spit. Chest x-rays can help detect the presence of tuberculosis in the lungs. 

This project utilizes convolutional neural networks (CNN) to learn from both tuberculosis-affected and normal chest x-ray images. The trained model can then predict whether a person has tuberculosis or not by taking their chest x-ray as input and making a prediction.

## Dataset

The dataset contains 4200 chest x-ray images in two categories: Normal and Tuberculosis. The metadata file provides the necessary information to read and organize the images. 

## How to Run the Program

1. Clone the repository and navigate to the project directory.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Download the dataset from [here](https://www.kaggle.com/tawsifurrahman/tuberculosis-tb-chest-xray-dataset).
4. Extract the dataset into a folder named `data`.
5. Run the `tb_classification.ipynb` notebook to train and evaluate the model.

## Results

This project uses binary classification to predict whether a chest x-ray image belongs to the normal or tuberculosis category. The trained model was able to achieve an accuracy of 87.57% on the test dataset. The classification report provides additional evaluation metrics such as precision, recall, and F1-score.

Since the dataset is imbalanced with more normal images than tuberculosis images, sample weighting was used to equalize the contribution from both classes during training. Due to this imbalance, the model may perform well in predicting one class, and thus we have only one neuron in the dense output layer.
