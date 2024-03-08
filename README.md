# job-matching
Job-Matching - A Neural Network Approach ( Deep Learning Project )

Introduction: Matching resumes to job descriptions is a time-consuming and challenging task for job seekers as well as the recruiters. The goal of this project is to develop a deep learning-based model that can accurately match resumes to job descriptions based on their content.​

Methodology:

Collected Dataset on our own
Dataset comprises of Resumes and Job Descriptions
Collection of Resumes was taken from Kaggle (https://github.com/florex/resume_corpus)
Job Descriptions are being generated using pre trained models like GPT, BERT
In order to fine tune the model we need to have resume and job description data
out of 29k, 4000 Resumes have been generated from ChatGPT API
Negative Sampling has been created which can help the model to differentiate.
Fine tuned the pre trained model Facebook's bart-large using the 4000 resume and job descriptions
Cosine Similarity helped us in labeling (matching/non-matching)
Median acted as Threshold in Labeling
Feature Extraction Using Word Embedding, TF-IDF, Word2Vec.
Built and evaluated different Models (BILSTM, LSTM, CNN, RNN)
Pre-Processing:

lowercasing the text
Removing Special Characters
We have not deleted the numbers as some of the skills consists numbers in it, experience
Limitations:

Faced an issue with API calls per minute
OPENAI API supports only 4000 approx. tokens for a single request - so we had to limit the job description length to 500 tokens
