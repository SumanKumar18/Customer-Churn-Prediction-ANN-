# 📊 Customer Churn Prediction Using Artificial Neural Networks (ANN)

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange?logo=tensorflow)
![Machine Learning](https://img.shields.io/badge/Focus-Machine%20Learning-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview

This project demonstrates customer churn prediction using an Artificial Neural Network (ANN) built with TensorFlow and Keras.

Customer churn prediction is a classification problem that aims to identify customers who are likely to stop using a service. This project uses a practice dataset of 1,000 customer records to demonstrate data preprocessing, neural network training, prediction, and model evaluation.

**Note:** The dataset is synthetically generated for practice and demonstration. It is not real customer data.

## 🎯 Objectives

- Generate a synthetic customer dataset.
- Preprocess numerical and categorical features.
- Split data into training and testing sets.
- Standardize input features.
- Build and train an ANN for binary classification.
- Predict whether a customer will stay or leave.
- Evaluate the model using accuracy.
- Visualize training and validation accuracy and loss using text-based curves.

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- TensorFlow
- Keras
- Scikit-learn

## 📂 Dataset Description

The project generates a dataset containing **1,000 customer records**.

| Feature | Description |
|---|---|
| `tenure` | Customer tenure, generated between 1 and 72 months |
| `monthly_bill` | Monthly bill amount, generated between 20 and 120 |
| `contract` | Contract type: Monthly or Yearly |
| `churn` | Target variable: `0` = stay, `1` = leave |

The synthetic churn labels are generated using probabilities influenced by contract type and customer tenure. Monthly-contract customers and customers with less than 12 months of tenure have higher assigned churn probabilities.

The dataset is generated within the notebook, so no external dataset download is required.

## 🧠 ANN Model Architecture

The neural network is built using TensorFlow/Keras Sequential API.

| Layer | Configuration |
|---|---|
| Input | Number of preprocessed input features |
| Hidden Layer 1 | 16 neurons, ReLU activation |
| Hidden Layer 2 | 8 neurons, ReLU activation |
| Output Layer | 1 neuron, Sigmoid activation |

### Model Configuration

- **Optimizer:** Adam
- **Loss Function:** Binary Crossentropy
- **Metric:** Accuracy
- **Epochs:** 20
- **Batch Size:** 32
- **Validation Split:** 20% of the training data

## ⚙️ Project Workflow

1. Generate a synthetic dataset containing customer tenure, monthly bill, and contract type.
2. Generate binary churn labels using predefined probabilities.
3. Convert categorical features into numerical columns using Pandas `get_dummies()`.
4. Separate the input features and target variable.
5. Split the dataset into 80% training data and 20% testing data.
6. Standardize the features using `StandardScaler`.
7. Build and compile the ANN.
8. Train the model for 20 epochs.
9. Predict churn probabilities for the test data.
10. Convert probabilities into binary predictions using a threshold of 0.5.
11. Calculate test accuracy.
12. Display training and validation accuracy and loss as text-based curves.

## 📈 Results

The model was trained for 20 epochs.

| Metric | Result |
|---|---:|
| Test Accuracy | 69.5% |
| Final Training Accuracy | Approximately 69.4% |
| Final Validation Accuracy | 67.5% |

The reported test accuracy is based on the generated synthetic dataset and the displayed execution output.

These results demonstrate the basic ANN classification workflow. They should not be interpreted as evidence of real-world customer churn prediction performance.

## 📉 Training Visualization

The notebook includes text-based curves for:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss

These curves show how the training metrics change across epochs.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Folder

```bash
cd Customer-Churn-Prediction
```

### 3. Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Open the Notebook

Open `Customer churn prediction -ANN.ipynb` using Jupyter Notebook or Visual Studio Code.

Run the notebook cells in order to generate the dataset, train the ANN, evaluate predictions, and display the training curves.

## 📋 Requirements

- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook or Visual Studio Code

## 🔮 Future Improvements

- Use a real-world customer churn dataset.
- Add precision, recall, F1-score, and a confusion matrix.
- Compare ANN performance with other classification algorithms.
- Tune the neural network architecture and hyperparameters.
- Improve model evaluation using cross-validation.
- Build an interface for entering customer details and predicting churn.

## 👨‍💻 Author

**Suman Kumar**

- GitHub: [SumanKumar18](https://github.com/SumanKumar18)
- LinkedIn: [Connect on LinkedIn](https://www.linkedin.com/in/sumank18)

---

⭐ If you find this project useful, consider giving the repository a star!
