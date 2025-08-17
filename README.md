# Medical-Transcript-Classification-and-Monitoring-using-DistilBERT-on-AWS
<img width="1121" height="611" alt="architecture" src="https://github.com/user-attachments/assets/2e376efd-6ccd-4807-8507-02ca5305c7f4" />
Project Overview
This project demonstrates an end-to-end AWS cloud architecture for training, deploying, and monitoring a Hugging Face transformer-based NLP model using Amazon SageMaker, with real-time data and model performance visualization in AWS QuickSight.
Main goal of this project is to solve a biomedical text classification problem by classifying medical transcripts into the correct diagnostic procedure category using the distilbert-base-uncased model fine-tuned on a curated dataset of medical transcriptions.
Key Features
Transformer Model Fine-Tuning
Used distilbert-base-uncased for 23-class medical transcript classification.
Applied custom class-weighted loss to address dataset imbalance.
Tokenization with Hugging Face AutoTokenizer for optimal text preprocessing.
AWS SageMaker Integration
Managed training, validation, and inference pipelines.
Leveraged Hugging Face Deep Learning Containers (DLCs) for seamless deployment.
Trained on ml.p3.2xlarge instances, deployed to ml.t2.medium endpoint.
Data Pipeline & Storage
All raw, preprocessed, and model artifacts stored in Amazon S3.
Preprocessed datasets split into training and validation sets for reproducibility.
Model Monitoring Dashboard (AWS QuickSight)
EDA Dashboard: Distribution of medical specialties, relationships, and word clouds of transcript context.
Model Performance Dashboard: Accuracy, precision, recall, F1-score, and prediction correctness comparisons between actual and predicted labels.
Dataset
Source: Medical Transcription Dataset (Kaggle)
Contains medical transcriptions across various specialties.
Reduced from 40 to 23 classes due to low-sample categories.
