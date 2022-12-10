## 11785-FakeNewsDetection

This is our project for the course 11-785: Introduction to deep learning. 

Authors: Adnan Lokhandwala, Benny Uhoranishema, Nihar Gaddam, Xiangjian(Aaron) Zeng


## The following tasks are performed:

#1) Document retrieval

Code: FEVER/FEVER_doc_retrieval.ipynb

An AllenNLP based Constituency Predictor extracts nouns from a claim, which is then used by Wikipedia API to extract the most relevant documents to a claim. Inspired by: https://github.com/aditya5558/BERT-FEVER-Task

#2) Sentence retrieval

Code: FEVER/FEVER_sentence_retrieval.ipynb

Evidence is retrived from the above documents by downloading the web pages from wikipedia, and encoding each sentences in each document with the Hugging Face Sentence Transformer. The encoded sentences are then compared with the encoded claim based on cosine similarity scores and the top 5 most relevant sentences are retrieved. Inspired by: https://towardsdatascience.com/bert-for-measuring-text-similarity-eec91c6bf9e1

#3) Claim verification

Code: LIAR-PLUS/Claim_Verification.ipynb

Uses a triple siamese BERT model which takes as input the claim, the evidence, the metadata of the post and the credibility of the author and outputs a true/false. Inspired by: https://github.com/manideep2510/siamese-BERT-fake-news-detection-LIAR
