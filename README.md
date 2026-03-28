SmartSpend: NLP-Driven Transaction Classifier
1. Project Overview
SmartSpend is a machine learning solution designed to automate the tedious task of financial categorization. In traditional banking apps, users must manually tag every purchase. This project leverages Natural Language Processing (NLP) to analyze transaction descriptions and automatically assign them to categories like "Food," "Transport," or "Utilities."
2. The Problem
Manual data entry is the primary reason people stop tracking their finances. By using a probabilistic model, SmartSpend removes this friction, turning raw text strings into structured financial data without human intervention.
3. Technical Architecture
The system is built using a Supervised Learning workflow:
Feature Extraction: Raw text is processed through a CountVectorizer. This converts human language into a "Bag-of-Words" numerical matrix.
Classification Engine: I implemented the Multinomial Naive Bayes algorithm. This model is ideal for text because it calculates the probability of a category based on word frequency.
Deployment Pipeline: Using a Scikit-Learn pipeline, the preprocessing and prediction stages are unified into a single, efficient command.
4. Core Logic Preview
The project uses a trained model to perform "inference." For example:
Input: "Starbucks Morning Coffee"
Process: Vectorization - Naive Bayes Probability Calculation
Output: Food & Dining
5. Setup & Installation
To run this project locally, ensure you have Python installed and follow these steps:
Clone the Repository
Install Dependencies
Execute the Classifier
6. Key Learnings
Vectorization: Understood how to map high-dimensional text data into numerical space.
Model Accuracy: Learned that even with a small dataset, Naive Bayes provides high accuracy for short-text classification.
Generalization: The model successfully identifies "Lyft" as "Transport" even if only "Uber" was present in the training data, proving the power of pattern recognition.

