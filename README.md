# Classifying-duplicate-questions-from-Quora-with-Keras
Used keras text_tokenizer and pad_sequences functions to preprocess the text data.

Used a Siamese network to predict whether the pairs are duplicated or not. 
The idea is to create a model that can embed the questions(sequence of words) into a vector.

We made use of keras layer_embedding and layer_lstm functions to define the part of the keras model that will embed the questions into a vector.

Further we used cosine similarity to measure the similarity between the questions which are in vector form.

Finally we designed a keras model in terms of its inputs and outputs and compile it. 
In the compilation phase we define our loss function and optimizer. We used Adam optimizer to minimize the logloss.

Encorporated tfruns package to hypertune the parameters for the keras model.

