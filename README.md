# House Price Prediction Using PyTorch

A beginner-friendly Machine Learning project that demonstrates how to build, train, evaluate, and save a Neural Network using **PyTorch** to predict house prices.

This project follows 20 practical steps, making it easier to understand the complete workflow of a basic regression model.

## Project Overview

The model predicts house prices based on three input features:

- **House Size** – Size of the house.
- **Number of Bedrooms** – Total number of bedrooms.
- **House Age** – Age of the house in years.

The predicted house price is expressed in **Lakhs**.

> **Note:** This project uses a small illustrative dataset for learning purposes. It is not intended for real-world property price estimation.

## Technologies Used

- Python
- PyTorch
- Google Colab
- Machine Learning
- Neural Networks
- Regression

## Model Architecture

The project uses a simple Feedforward Neural Network.

```text
Input Layer:       3 Features
       |
       v
Hidden Layer 1:   16 Neurons
       |
      ReLU
       |
       v
Hidden Layer 2:    8 Neurons
       |
      ReLU
       |
       v
Output Layer:      1 Neuron
       |
       v
Predicted House Price
```

## Project Workflow – 20 Practical Steps

1. Import Required Libraries
2. Create Dataset (Input Features)
3. Create Target Values
4. Understand Dataset Shape
5. Combine Dataset
6. Split Dataset (Training & Testing)
7. Separate Training and Testing Features
8. Normalize the Data
9. Create DataLoader
10. Create Neural Network Model
11. Initialize the Model
12. Define Loss Function
13. Define Optimizer
14. Training Loop (Epochs)
15. Model Evaluation (Testing)
16. Make New Predictions
17. Save Trained Model
18. Save Normalization Values
19. Load Trained Model
20. Predict Using Loaded Model

## Training Configuration

| Parameter | Value |
|---|---|
| Input Features | 3 |
| Hidden Layers | 2 |
| Hidden Layer Neurons | 16, 8 |
| Output Neurons | 1 |
| Activation Function | ReLU |
| Loss Function | Mean Squared Error (MSE) |
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Epochs | 500 |
| Batch Size | 2 |
| Train/Test Split | 80% / 20% |

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
```

### 2. Navigate to the Project

```bash
cd YOUR_REPOSITORY_NAME
```

### 3. Install PyTorch

```bash
pip install torch
```

### 4. Open the Notebook

Open the `.ipynb` notebook using either:

- Google Colab
- Jupyter Notebook
- Visual Studio Code with Jupyter extension

For Google Colab, upload the notebook and execute the cells sequentially from Step 1 to Step 20.

## Making a Prediction

The notebook demonstrates a prediction using the following sample input:

```python
new_house = torch.tensor(
    [[1500, 3, 5]],
    dtype=torch.float32
)
```

This represents:

- House Size: 1500
- Bedrooms: 3
- House Age: 5 years

The trained model returns a predicted house price in Lakhs.

## Saving and Loading the Model

The project demonstrates how to save and reuse the trained model.

**Model weights:**

```text
house_price_model.pth
```

**Normalization values:**

```text
normalization.pth
```

Both files are required to restore the trained model and correctly preprocess new input data.

## Learning Outcomes

By completing this project, you will understand:

- How to prepare datasets using PyTorch tensors.
- How to split data into training and testing sets.
- Why data normalization is important.
- How to create a Neural Network using `nn.Module`.
- How activation functions work.
- How to train a model using an optimizer and loss function.
- How to evaluate a regression model.
- How to make predictions using new input data.
- How to save and load trained model parameters.
- How to reuse preprocessing values during inference.

## Future Improvements

- Use a larger, real-world housing dataset.
- Add more relevant house features.
- Experiment with different neural network architectures.
- Compare model performance using additional evaluation metrics.
- Build a simple interface for house price predictions.

## Author

**Vasireddy Srimanth**

Android Developer | Mobile Engineering | AI & Machine Learning Enthusiast

---

⭐ If you find this project useful for learning PyTorch and Machine Learning, consider giving the repository a star!
