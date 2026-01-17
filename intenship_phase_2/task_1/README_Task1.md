# Task 1: News Topic Classifier

This project builds a **News Topic Classifier** using a pre-trained **BERT** model to categorize news headlines into four major topics: **World, Sports, Business, and Sci/Tech**.

## 📌 Objective
To fine-tune a Transformer-based model (BERT) for text classification (`ag_news` dataset) and deploy a simple interactive interface for real-time predictions.

## 📂 Dataset
**Source**: [AG News Dataset](https://huggingface.co/datasets/ag_news) (via Hugging Face Datasets library)

The dataset contains 4 classes:
1.  **World**
2.  **Sports**
3.  **Business**
4.  **Sci/Tech**

## 🛠️ Tech Stack
-   **Python 3.8+**
-   **Transformers (Hugging Face)**: For loading `bert-base-uncased` and `Trainer` API.
-   **Datasets**: For loading `ag_news`.
-   **Evaluate**: For computing accuracy metrics.
-   **Scikit-learn**: For classification reports and confusion matrices.
-   **Matplotlib & Seaborn**: For visualization.
-   **Gradio**: For the web-based demo interface.

## 🚀 How to Run

1.  **Install Dependencies**:
    ```bash
    pip install transformers datasets evaluate accelerate streamlit gradio scikit-learn matplotlib seaborn
    ```

2.  **Run the Notebook**:
    Open `task_1_News_Topic_Classifier .ipynb` in Jupyter Notebook, Google Colab, or VS Code.

3.  **Execution Steps**:
    -   **Data Loading**: Automatically downloads `ag_news`.
    -   **Preprocessing**: Tokenizes text using BERT tokenizer (max length 128).
    -   **Training**: Fine-tunes BERT for 4-class classification.
    -   **Evaluation**: Displays Accuracy, Precision, Recall, F1-score, and Confusion Matrix.
    -   **Demo**: Launches a Gradio app to test custom headlines.

## 🧠 Model Architecture
-   **Base Model**: `bert-base-uncased`
-   **Task**: Sequence Classification (4 labels)
-   **Tokenizer**: BERT Tokenizer (WordPiece)

## 📊 Results & Visualization
The notebook provides:
-   **Classification Report**: Detailed metrics per class.
-   **Confusion Matrix**: Heatmap showing misclassifications.
-   **Interactive Demo**: Type a headline (e.g., *"Nvidia releases new GPU"*) and get the predicted category.
