# AI-ML-Internship-DevelopersHub
This repository showcases the projects and technical milestones completed during my AI/ML Engineering Internship at DevelopersHub Corporation. The portfolio covers the full machine learning lifecycle, from exploratory data analysis to fine-tuning large language models.


🛠️ Detailed Task Summaries

Task 1: Iris Species Visualization


Objective: To load, inspect, and visualize the classic Iris dataset to understand relationships between physical flower measurements and species.


Dataset: Iris Dataset.

Models/Tools: Pandas, Matplotlib, and Seaborn.

Key Findings: Exploratory Data Analysis (EDA) revealed that petal dimensions provide a significantly clearer separation between species than sepal measurements.

Task 2: Short-Term Stock Price Prediction

Objective: To build a regression model that predicts the next day's closing price using historical market data.

Dataset: Stock market data retrieved via the yfinance library.

Models: Random Forest Regressor.

Key Findings: The model successfully tracked general market movements. By shifting the "Close" price to create a target for the next day, the Random Forest model was able to handle non-linear market fluctuations effectively.

Task 3: Heart Disease Prediction

Objective: To build a model predicting heart disease risk based on patient health metrics.


Dataset: Heart Disease UCI Dataset.


Models: Logistic Regression and Decision Trees.


Key Findings: Feature importance analysis highlighted that age and maximum heart rate are critical indicators for risk prediction. The model was evaluated using ROC curves and confusion matrices to ensure medical diagnostic reliability.
+1

Task 4: General Health Query Chatbot
Objective: To design a Generative AI chatbot providing general health information using a professional medical assistant persona.

Model: zephyr-7b-beta via Hugging Face Inference API.

Key Findings: Successfully implemented a hybrid safety architecture. A custom rule-based filter identified 100% of emergency queries (like chest pain), while prompt engineering ensured the LLM maintained a non-diagnostic, supportive tone for general queries.

Task 5: Mental Health Support Chatbot

Objective: To develop a specialized AI that provides empathetic and gentle responses for emotional wellness.

Dataset: EmpatheticDialogues (Facebook AI).

Model: Fine-tuned distilgpt2 using Hugging Face's Trainer API.

Key Findings: Fine-tuning allowed the model to move beyond simple pattern matching to generate mood-responsive interactions. To fix technical challenges like repetition loops, I implemented specific repetition penalties (1.5) and n-gram filters.

🏗️ Repository Organization

In accordance with the internship guidelines, each task is organized as follows:


Jupyter Notebooks: Containing modular, commented code and step-by-step explanations.
+1

Visualizations: Charts and plots (Scatter, Histograms, Box plots, ROC curves) illustrating findings.


Documentation: Task-specific README files summarizing individual project insights.

📅 Submission & Contact

Internship: AI/ML Engineering DevelopersHub Corporation.


Submission Date: 23rd December 2025.


Format: GitHub Repository submitted via Google Classroom.

How to Use This Repo:

Navigate to the individual task folders to view the source code.

Run the .ipynb files in Google Colab or a local Jupyter environment.

For Task 5, use the Gradio interface code to interact with the fine-tuned model.



