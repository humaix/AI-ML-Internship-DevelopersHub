# Multimodal Housing Price Prediction

This project implements a multimodal machine learning model to predict housing prices using both structured tabular data (number of bedrooms, bathrooms, square footage) and unstructured image data (house photos).

## 📌 Objective
To combine visual features extracted via a Convolutional Neural Network (CNN) with tabular features processed by a Multilayer Perceptron (MLP) to improve price prediction accuracy.

## 📂 Dataset
**Source**: [SoCal House Prices and Images Dataset](https://www.kaggle.com/datasets/ted8080/house-prices-and-images-socal/data)

The dataset consists of:
-   **`socal2.csv`**: Tabular data containing features like address, city, bedrooms, bathrooms, sqft, and price.
-   **`socal_pics/`**: A folder containing images of the houses corresponding to the rows in the CSV.

*(Note: The dataset was originally mounted from Google Drive or downloaded locally. Ensure the `dataset` folder is present in the root directory before running.)*

## 🛠️ Tech Stack
-   **Python 3.8+**
-   **PyTorch**: For building the multimodal neural network.
-   **Torchvision**: For pre-trained ResNet models and image transformations.
-   **Pandas & NumPy**: For data manipulation.
-   **Scikit-learn**: For data splitting and preprocessing (StandardScaler, OneHotEncoder).
-   **Gradio**: For the interactive web interface.

## 🚀 How to Run

1.  **Install Dependencies**:
    The notebook allows for automatic installation, or you can run:
    ```bash
    pip install torch torchvision pandas scikit-learn matplotlib seaborn gradio pill
    ```

2.  **Prepare Data**:
    Ensure your directory structure looks like this:
    ```text
    Task2/
    ├── dataset/
    │   ├── socal2.csv
    │   └── socal2/
    │       └── socal_pics/
    ├── task_3_final.ipynb
    └── README.md
    ```

3.  **Run the Notebook**:
    Open `task_3_final.ipynb` in Jupyter Notebook or VS Code and execute all cells.

## 🧠 Model Architecture
The model consists of two branches:
1.  **Image Branch**: A pre-trained **ResNet18** (with frozen weights initially) extracts features from house images.
2.  **Tabular Branch**: A simple Feed-Forward Neural Network (MLP) processes numerical input (Bed/Bath/Sqft).
3.  **Fusion Layer**: The outputs of both branches are concatenated and passed through a final regression head to predict the price.

## 📊 Evaluation
The model is evaluated using:
-   **MAE** (Mean Absolute Error)
-   **RMSE** (Root Mean Squared Error)

## 🖥️ Demo
A **Gradio Interface** is included at the end of the notebook. It allows you to upload a house image and enter features to get a real-time price prediction.
