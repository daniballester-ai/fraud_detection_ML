# 📊 Credit Card Fraud Detection Project

Welcome to the **Credit Card Fraud Detection** project! In this repository, we tackle the challenge of detecting fraudulent transactions using machine learning techniques. Since the dataset is highly imbalanced—frauds account for only **0.172%** of all transactions—we’ve used **SMOTE** (Synthetic Minority Over-sampling Technique) to address this issue and improve model performance. Let’s dive in! 🚀

## 🚀 Project Overview

The main objective of this project is to build an efficient predictive model to detect fraudulent credit card transactions while minimizing false positives. The model uses SMOTE to handle the class imbalance, ensuring that our model gets sufficient exposure to fraud cases.

Key techniques used:
- **Data preprocessing**
- **SMOTE for class balancing**
- **Feature engineering**
- **Machine learning algorithms**
- **Model evaluation metrics**

## 🗂 Dataset

The dataset consists of **284,807 credit card transactions**, with **492 fraud cases**. Each transaction is represented by several anonymized features, most of which have been derived using PCA (Principal Component Analysis). Only the `Time` and `Amount` features remain untransformed, along with the `Target` feature which indicates fraud.

You can download the dataset (`transferencias.csv`) from this [Google Drive link](https://drive.google.com/file/d/1cOAxzQf6j03mXGrmbDFbcUCT94g5bHR/view?usp=sharing) 💾.

## 📁 Features

Here’s an overview of the key features in the dataset:

- `Timestamp`: Transaction time
- `pais`, `cidade`, `bairro`, `cep`, `ip`: Geographic and network information
- `dia`, `hora`, `minuto`: Temporal transaction details
- `valor`: The amount of the transaction
- `antecedentes`: User's transaction history
- `reclamacoes`: Number of user complaints
- `qtd_trans`: Total number of user transactions
- `navegador`, `android`, `ios`: Browser and OS details
- `Target`: The label indicating fraud (1 for fraud, 0 for non-fraud)

## ⚙️ Handling Class Imbalance with SMOTE

Given the imbalance in fraud cases, we applied **SMOTE** to generate synthetic samples of the minority class (fraud). This helped improve model training by providing the algorithm with more instances of fraudulent transactions, balancing the dataset for better learning.

## 📚 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/fraud_detection_project.git
   cd fraud_detection_project
   ```

2. Download the dataset from the link above and place it in the project directory.

3. Run the Jupyter notebook `fraud_detection_ML.ipynb` to explore the dataset, apply SMOTE, and train the machine learning model.

## 🔍 Evaluation

We’ll evaluate the model performance based on several metrics like:

- **Precision**: How many predicted frauds were actual frauds?
- **Recall**: How many of the actual frauds were detected?
- **F1 Score**: A balance between precision and recall.

## 🛠 Future Enhancements

- Explore alternative techniques for handling class imbalance (e.g., under-sampling, different sampling strategies).
- Test additional machine learning models and ensemble methods.
- Fine-tune hyperparameters for further improvements.

## 🤝 Contributing

Feel free to contribute by forking the repo, making changes, and submitting pull requests! We appreciate your input to improve this project.

## 📧 Contact

For any questions or suggestions, feel free to reach out via [danielleballester@gmail.com] or submit an issue in the repository.

Happy Coding! 🎉
