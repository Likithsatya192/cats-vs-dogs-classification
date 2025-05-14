# Cat vs Dog Image Classifier

This project is a deep learning image classifier that distinguishes between images of cats and dogs. The model was built and trained in Google Colab using TensorFlow and Keras, and the dataset was sourced from Kaggle.

## Dataset
- **Source:** [Kaggle Dogs vs Cats Dataset](https://www.kaggle.com/datasets/salader/dogs-vs-cats)
- **Training Images:** 20,000
- **Validation Images:** 5,000
- **Classes:** Cat, Dog

## Environment
- **Platform:** Google Colab
- **Frameworks:** TensorFlow, Keras
- **Data Source:** Kaggle API

## Model Architecture
The model is a Convolutional Neural Network (CNN) with the following layers:
- 3x Conv2D layers with increasing filters (32, 64, 128), each followed by BatchNormalization and MaxPooling2D
- Flatten layer
- Dense layer with 128 units + Dropout
- Dense layer with 64 units + Dropout
- Output Dense layer with 1 unit (sigmoid activation)

## How to Run
1. Download the notebook (`cat_vs_dog.ipynb`).
2. Upload your Kaggle API key (`kaggle.json`) to Colab.
3. Run the notebook cells in order. The notebook will automatically download and extract the dataset from Kaggle.
4. Training and evaluation will be performed in Colab.

## Example Usage
After training, you can use the model to predict whether a new image is a cat or a dog by loading the model and passing a preprocessed image through it. See the notebook for example inference code.

## Notes
- The model may be further improved with data augmentation, hyperparameter tuning, or more advanced architectures.
- The notebook demonstrates the full workflow: data loading, preprocessing, model building, training, and evaluation.

---
**Author:** Likith Sagar
