# Laptop Price Prediction using DANCS (Deep Artificial Neural Costing System)

This project implements **DANCS**, a Deep Artificial Neural Costing System designed to predict laptop prices based on key specifications such as RAM, CPU, storage type, GPU, screen size, and operating system. The system uses machine learning to provide accurate price estimation in Philippine Pesos (PHP).

---

## 📁 Project Structure

```
root/
├── Laptop_DANCS.ipynb          # Jupyter notebook for training and analysis
├── Updated_laptop_dancs.py     # Main Python script for model building and inference
├── raw_laptop_price_php.csv    # Raw dataset containing original laptop listings
├── cleaned_laptop_data.csv     # Cleaned dataset after preprocessing
├── train_data.csv              # Training data
├── valid_data.csv              # Validation data
├── test_data.csv               # Testing data
```

---

## 🧠 Features

- Cleans and preprocesses raw laptop specification data.  
- Encodes categorical variables such as CPU, GPU, and OS.  
- Trains a deep neural network to predict laptop prices.  
- Evaluates performance using separate training, validation, and testing splits.  
- Supports both Jupyter-based experimentation and standalone script execution.

---

## ⚙️ Requirements

Install dependencies before running the code:

```bash
pip install pandas numpy scikit-learn tensorflow matplotlib
```

Optional for Jupyter notebook usage:

```bash
pip install jupyter
```

---

## 🚀 How to Run

### Option 1: Using the Notebook
Open the notebook and run all cells:

```bash
jupyter notebook Laptop_DANCS.ipynb
```

### Option 2: Using the Python Script
Execute the standalone Python script for training or prediction:

```bash
python Updated_laptop_dancs.py
```

---

## 🧾 Dataset Description

The dataset contains the following attributes:

| Feature | Description |
|----------|--------------|
| Inches | Screen size (diagonal) |
| Ram_GB | Installed memory (in GB) |
| Laptop Weight_Kg | Weight of the laptop |
| Company | Laptop manufacturer |
| TypeName | Category (Budget, Performance, Premium) |
| Screen Resolution (PPI) | Pixel density |
| CPU | Processor type (Entry-Level, Mid-Range, High-End) |
| Storage | Type and size of storage (SSD/HDD) |
| GPU | Integrated or Dedicated graphics |
| OS | Operating system type |
| Price (PHP) | Target variable |

---

## 📊 Model Overview

The DANCS model is a **deep learning regression model** that:
- Uses dense layers with ReLU activation.
- Applies dropout regularization to prevent overfitting.
- Trains using Mean Squared Error (MSE) loss and Adam optimizer.

Performance is evaluated using metrics such as:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 📈 Example Output

After training, the system outputs:
- Model summary
- Loss/accuracy plots
- Evaluation metrics on test data
- Optional prediction samples comparing actual vs. predicted prices

---

## 🧑‍💻 Authors

**Developed by:**  
A 3rd-Year College Research Team, Holy Angel University  
**Project Title:** *Deep Artificial Neural Costing System for Laptop Price Prediction*

---

## 🪪 License

This project is for academic and research purposes only.
