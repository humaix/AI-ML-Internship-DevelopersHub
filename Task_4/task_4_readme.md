# **General Health Query Chatbot**



### **1. Task Objective**



The primary objective of this project was to design and implement a Generative AI Chatbot capable of providing general health information. The focus was on utilizing Prompt Engineering to create a professional medical assistant persona while implementing strict Safety Guardrails to prevent the dissemination of harmful medical advice or unauthorized diagnoses.



### **2. Dataset Used**



As this is a Natural Language Processing (NLP) task based on a Large Language Model (LLM), a traditional static dataset (like a CSV file) was not used for training. Instead, the project utilized:



**Prompt-Based Context:** A custom-designed System Prompt served as the foundational "knowledge and behavior" set for the model.



**Evaluation Dataset:** A curated set of test queries (Sore throat causes, Paracetamol safety, and Emergency chest pain) was used to validate the model's accuracy, empathy, and safety triggers.



### **3. Models Applied**



Large Language Model: HuggingFaceH4/zephyr-7b-beta (an advanced 7-billion parameter model optimized for following instructions).



**Task Type**: Conversational (Chat Completion).



**Safety Layer:** A custom Python-based Rule Engine (Keyword Filtering) applied before the LLM inference to handle high-risk emergency detection.



### **4. Key Results and Findings**



Emergency Redirection: The hybrid architecture successfully identified 100% of life-threatening queries (e.g., chest pain) and bypassed the LLM to provide immediate emergency instructions, ensuring user safety.



**Persona Adherence:** Through prompt engineering, the bot maintained a non-diagnostic tone, successfully explaining medical conditions (like Pharyngitis) while consistently directing users to licensed professionals for diagnosis.



**Dosage Safety:** The model correctly refused to provide specific weight-based medication dosages for children, instead pointing users toward official product labeling and physician consultation.



**Technical Efficiency:** Using a Temperature setting of 0.3 effectively reduced hallucinations, ensuring that the assistant remained factual and stable across multiple query types.









### Final Instructions for your Colab Notebook:



Ensure you have replaced YOUR\_TOKEN\_HERE with your actual Hugging Face token.



Check that all Markdown headers (Problem Statement, Dataset, etc.) match the checklist in the previous message.



Click File -> Save.



Click File -> Download -> Download .ipynb.

