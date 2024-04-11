# SemEval 2010 Task 8: Relation Extraction

We perform Relation Extraction on SemEval 2010 Task 8 dataset. The paper for this work is provided in the same folder.

Group Members:
1. Mohammed Mehdi Patel
2. Antas Singh
3. Ayush Garg
4. Nilakhi Das

The folder contains two python notebooks corresponding to our two approaches to perform relation extraction:
1. Approach_1.ipynb (SVM)
2. Approach_2.ipynb (Bi-LSTM)

Both the notebooks were prepared on Google Colab. The cells to mount Google Drive are commented. If you want to run these notebooks on Google Colab, uncomment those cells.

Before running the python notebooks make sure to install the required libraries. The install statements are present in the first line of each notebook. Running the notebooks from start to end will take a lot of time, so if you want to directly test our model by providing some input, then you can run the last few cells of the notebooks. Instructions for the same are given in the notebook. Also, donwload the following files and put them in the project root directory before running those cells:

1. SVM model: https://drive.google.com/file/d/11HIz7mwrUHDYenGGVoI_9YP2ztDPwAYc/view?usp=sharing
2. Bi-LSTM model: https://drive.google.com/file/d/1AFDLlkODLQfYRT7OOBcSfLMdfU-lvQ4h/view?usp=sharing
3. Word Embeddings for SVM model: https://drive.google.com/file/d/1KCvnf4-bLDSmAT_4CMd0YBoYM02mFr-X/view?usp=sharing


The training data is in `SemEval2010_task8_training` folder and testing data is in `SemEval2010_task8_testing_keys` folder. `tfidf_vectorizer.joblib` is our tf-idf vectorizer that we use for generating features for the SVM model. `tokenizer.kv` is a word index used by the Bi-LSTM model.

Code Attributions:
- To get some preprocessing code: https://github.com/sahitya0000/Relation-Classification/tree/master
- To create word embeddings: https://www.tensorflow.org/text/tutorials/word2vec
- To create model and word index: https://keras.io/
- To use NLP techniques to generate features: https://spacy.io/usage