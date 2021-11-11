# SST_BERT-SEMEVAL_TASK1
# Semantic-Shift-Tracing-by-Clustering-in-Embedding-Space
The goal of the Shared Task (https://competitions.codalab.org/competitions/20948), is to trace the semantic shifts of words over the given corpora. This includes two tasks:
Task 1: Binary classification
Given two corpora C1 and C2 (for time periods t1 and t2), for a set of target words, decide which words lost or gained senses between t1 and t2, and which ones did not; as annotated by human judges.

Task 2: Ranking
Given two corpora C1 and C2, rank a set of target words according to their degree of lexical semantic change between t1 and t2, as annotated by human judges. A higher rank means stronger change.

The proposed approach uses K-means clustering over contextualized BERT embeddings to detect whether the sense of a given target word has changed/not(Task 1). Further, these clusters are used to derive the ranking of the target words, which defines the degree of the semantic divergences (Task 2).

The code is available in the Colab notebook: https://colab.research.google.com/drive/1AFTzeNwbsDuf_CK_l32leg2KTQl--rj6

Our paper is now available at https://arxiv.org/abs/2010.00857

## Usage Instructions

The datasets can be downloaded from [here](https://competitions.codalab.org/competitions/20948#learn_the_details-data).
If using colab notebook, the datasets should be stored in Google Drive (The Corpus texts, C1 and C2 and the target txts).
