# Smart-Subject-Email-Line-Generation-with-Word2Vec
Smart Subject Email Line Generation with Word2Vec
This repository contains the code from the article titled "Smart Subject Email Line Generation with Word2Vec", authored by me, and published on Analytics Vidhya. The project demonstrates how to generate subject lines for emails based on their body text using Word2Vec embeddings and cosine similarity for semantic search.

Read the full article here: https://www.analyticsvidhya.com/blog/2024/08/smart-subject-email-line-generation-with-word2vec/

Project Overview
In this project, we use:

Word2Vec: To create vector embeddings of email bodies.

Cosine Similarity: To compute the similarity between the embeddings of different emails and find the most semantically similar email body.

Sklearn: For train-test splitting and performance evaluation.

NLTK: For tokenization of email body text.

Key Steps

Data Preprocessing: Emails are tokenized and converted to lowercase. Missing values in email_body and subject_line are handled.

Word2Vec Embeddings: A Word2Vec model is trained on the email body texts to capture the semantic meaning of words.

Semantic Search: When a new email body is provided, its vector representation is compared against the training email body embeddings to find the most similar one. The corresponding subject line of the matched email is returned as the predicted subject line.

Model Evaluation: We evaluate the model by comparing the cosine similarity between the predicted and actual subject lines for test emails.

References
Original article: Smart Subject Email Line Generation with Word2Vec
