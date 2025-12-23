# **README: Mental Health Support Chatbot**





#### **1. Task Objective**

The primary objective of this project is to develop a specialized conversational AI that provides supportive, empathetic, and gentle responses for users experiencing stress, anxiety, or emotional distress. Unlike general-purpose chatbots, this model is specifically fine-tuned to recognize emotional contexts and respond in a way that validates the user's feelings and promotes emotional well-being.


**"Note: The Gradio interface is designed for interactive use in Google Colab. If it does not render on GitHub, please run the notebook in Colab to test the chatbot's empathetic responses."**


#### **2. Dataset Used**



**Source:** The EmpatheticDialogues dataset (Facebook AI).



**Description**: A large-scale dataset containing approximately 25,000 conversations grounded in a wide range of emotional situations.



**Key Feature:** Each dialogue is paired with one of 32 emotion labels (e.g., anxious, lonely, proud, sentimental), allowing the model to learn nuanced emotional associations rather than just generic text patterns.



#### **3. Models Applied**



**Base Model:** distilgpt2 (Distilled GPT-2).



**Why DistilGPT2?:** It is a lightweight version of GPT-2 with 82 million parameters, making it roughly 33% smaller and twice as fast while retaining over 95% of the original model's performance. Its compact size makes it ideal for deployment on resource-constrained environments like Google Colab.



**Fine-Tuning Framework:** Hugging Face Trainer API.



**Deployment Interface:** Gradio web interface, providing an accessible and interactive chat experience.



#### **4. Key Results and Findings**



**Improved Conversational Quality:** Models trained on this dataset are consistently perceived as more empathetic by human evaluators compared to models trained solely on large-scale general internet data.



**Emotional Context Awareness:** Through fine-tuning, the model moved beyond simple pattern matching to generate mood-responsive interactions that align with the user's stated emotional state.



**Optimized Generation:** To resolve common issues in smaller models (like repetition loops), the implementation successfully utilized repetition penalties (1.5) and no-repeat n-gram filters, resulting in more coherent and diverse dialogue.



**Accessibility:** The project demonstrates that affordable, smaller-scale models can effectively provide "safe space" digital support, particularly useful for users who prefer the anonymity of an AI agent over human interaction for sensitive topics.



**Suggested Queries to Try**

**Use these prompts to test the bot's empathetic response patterns:**



"I've been feeling really overwhelmed with my studies lately."



"I'm so excited! I finally got the job I was interviewing for."



"I feel a bit lonely since moving to this new city."



"I'm worried I might have let my friend down today."


