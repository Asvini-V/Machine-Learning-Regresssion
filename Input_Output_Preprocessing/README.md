📌 Project Title

Input and Output Preprocessing in Machine Learning using SVR

📖 Project Overview

This repository demonstrates input and output preprocessing techniques using Support Vector Regression (SVR). The project focuses on how preprocessing should be handled consistently during training and deployment phases.

📂 Folder Structure & Explanation
1️⃣ Input Preprocessing Only (SVR)

This folder contains two sets of SVR implementations, both using StandardScaler for input preprocessing.

Set 1:

Input features are scaled before training the SVR model

During deployment, the same preprocessing is manually applied again to the input

Only the trained SVR model is saved

Set 2:

Input features are scaled before training

Both the SVR model and the fitted StandardScaler are saved using pickle

During deployment, both are loaded to ensure consistent preprocessing

2️⃣ Input and Output Preprocessing (SVR)

In this approach:

Both input features and output target are scaled before training the SVR model

During testing/deployment:

Input data is scaled using the saved scaler

Predictions are generated on the scaled output

Inverse transformation is applied to convert predictions back to the original scale
