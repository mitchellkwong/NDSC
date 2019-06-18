## Overview
A transfer learning model was built to classify paired text and image data. 
(More details in the report) As the competition was hosted on kaggle, the code was broken up into several notebooks to keep within kaggle's memory, storage and runtime limitations.

## Source Code
### combined-meta-model
This notebook contains the training of the meta classifier described in the project report.

### mobile-nlp-data
This notebook contains sample code that handles the preprocessing of text data using the spaCy library for NLP. A variant of word embedding is carried out in which each word is represented as a vector, and each piece of text data is represented as the mean of the word vectors composing the text.
(More accurately, the mean of token vectors are averaged)

### nlp-model
This notebook handles the pre-training of the nlp model before its integration into the meta classifier (as described in the report). Time-efficient and effectiveness motivated the use of early stopping and model checkpointing to tackle overfitting.
