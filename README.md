# 🎮 League of Legends Match Predictor

A machine learning project that predicts the outcome of League of Legends matches using in-game statistics, built with a **PyTorch logistic regression model**.

Developed as the final project for the **IBM AI Engineering Professional Certificate** (Introduction to Neural Networks and PyTorch course).

---

## 📌 Project Overview

League of Legends, a popular multiplayer online battle arena (MOBA) game, generates extensive data from matches. This project applies machine learning to that data to predict whether a team will win or lose a match, based on various in-game statistics.

---

## 🏗️ Model Architecture & Approach

The project builds a complete machine learning pipeline around a **logistic regression model implemented in PyTorch**:

1. **Data Preparation**
   - Loading and preprocessing the League of Legends match dataset.
   - Splitting data into training and test sets.
   - Feature scaling using `StandardScaler`.

2. **Logistic Regression Model**
   - Built using PyTorch's `nn.Module`.
   - Uses a linear layer followed by a sigmoid activation function for binary classification (win/loss).

3. **Model Training**
   - Trained using gradient descent with a binary cross-entropy loss function.
   - Trained over multiple epochs, tracking loss at each step.

4. **Optimization**
   - L2 regularization (Ridge Regression) applied to reduce overfitting and improve generalization.

5. **Evaluation & Visualization**
   - Confusion matrix and classification report to assess model performance.
   - ROC curve to visualize the trade-off between sensitivity and specificity.

6. **Model Persistence**
   - Trained model saved using `torch.save` and reloaded using `torch.load` to confirm consistent performance.

7. **Hyperparameter Tuning**
   - Testing multiple learning rates to identify the optimal configuration for best test accuracy.

8. **Feature Importance**
   - Extracting model weights to understand which in-game statistics most strongly influence match outcomes.

---

## 🧰 Tech Stack

- **Language:** Python
- **Deep Learning Framework:** PyTorch
- **Data Handling:** Pandas, NumPy
- **Preprocessing & Metrics:** Scikit-learn
- **Visualization:** Matplotlib
- **Environment:** Jupyter Notebook

---

## 📊 Workflow

1. **Data Loading & Preprocessing** — Load match data, split into features/target, scale features.
2. **Model Definition** — Logistic regression model built with PyTorch.
3. **Training** — Model trained using gradient descent over multiple epochs.
4. **Optimization** — L2 regularization applied to improve generalization.
5. **Evaluation** — Confusion matrix, classification report, and ROC curve analysis.
6. **Model Saving/Loading** — Persisting the trained model for reuse.
7. **Hyperparameter Tuning** — Testing different learning rates for best performance.
8. **Feature Importance** — Analyzing which features most influence predictions.

---

## 📈 Results

- The logistic regression model successfully predicts match outcomes based on in-game statistics.
- L2 regularization improved model generalization and reduced overfitting.
- Confusion matrix and ROC curve confirm solid classification performance.
- Feature importance analysis identifies the key statistics that most influence whether a team wins or loses.

---

## 🚀 How to Run

1. Clone this repository.
2. Open `Final Project League of Legends Match Predictor.ipynb` in Jupyter Notebook or Google Colab.
3. Install the required libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib torch torchvision torchaudio
   ```
4. Run all cells in order (**Kernel → Restart & Run All**).
5. View outputs including training loss, confusion matrix, ROC curve, and feature importance chart.

---

## 🎓 Acknowledgment

This project was completed as part of the **IBM AI Engineering Professional Certificate** on Coursera, developed by IBM Skills Network.

---

## 👩‍💻 Author

**Umaira Tahir**
