# Sentiment Analysis AI System: Deployment and Performance Study

## Project Overview
This project focuses on the development and deployment of a Natural Language Processing (NLP) system designed to classify textual opinions into three primary categories: Positive, Negative, and Neutral. The system provides an automated alternative to manual sentiment classification, optimized for handling large-scale textual datasets such as product reviews and social media feedback.

## Performance and Evaluation Metrics
The model was trained and validated using a rigorous machine learning pipeline, achieving the following technical results:
* Accuracy Score: 85.44%
* Classification Algorithm: Logistic Regression
* Feature Extraction: TF-IDF (Term Frequency-Inverse Document Frequency)
* Hyperparameters: N-gram range of (1,2) to capture both individual words and contextual phrases.
* Dataset: Amazon Fine Food Reviews (over 560,000 samples).

## Technical Implementation
The system architecture consists of two integrated components:
1. The Machine Learning Pipeline: Developed using Python, utilizing NLTK for text preprocessing (tokenization, stopword removal, and cleaning) and Scikit-learn for model training.
2. The Web Interface: A Flask-based application that serves as the bridge between the trained model and the user interface.
3. External Access: Implementation of Ngrok for public tunneling, allowing the application to be accessible via a public URL during the development and testing phases.

## System Components
* Text Preprocessing: Automated logic for case folding, URL removal, and lemmatization to ensure high data quality.
* Prediction Engine: Backend logic that transforms user input into numerical vectors using the TF-IDF vectorizer before passing it to the Logistic Regression model.
* Responsive UI: A web dashboard that provides real-time visual feedback based on the sentiment classification results.

## Repository Structure
* Sentiment_Analysis_Pipeline.ipynb: The primary Jupyter Notebook containing the training logic and the Flask server code.
* Sentiment-Analysis-Technical-Report.pdf: Comprehensive technical documentation detailing the methodology and performance matrices.
* templates/: Directory containing the HTML templates for the web application's frontend.

