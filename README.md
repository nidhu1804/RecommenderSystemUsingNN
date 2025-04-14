Amazon Toy Product Recommender System Using NLP and Neural Network:

This project implements product recommender system using amazon's toy product dataset. Starting with data exploration, cleaning and preprocessing. Firstly, the numerical and categorical features, and then the textual features using Natural Language Processing (NLTK Library). 

The models are built such that it classifies products into one of the top 20 most frequent categories. It starts by filtering the dataset to include only entries from the top 20 classes. 

Model 1 builds a simple Recurrent Neural Network (RNN) using Keras to classify products based on their names. It starts by encoding product names into numerical labels and target categories using LabelEncoder, and splits the dataset into training, validation, and test sets. The target labels are one-hot encoded for categorical classification,  The model architecture includes an embedding layer for product name embeddings, followed by a SimpleRNN layer and a dense output layer with softmax activation for multiclass classification. The model is trained on the encoded product names, and performance is evaluated on the test set. Finally, training history is visualized through loss and accuracy plots.

Model 2 implements an LSTM-based deep learning model to classify products based on their descriptions (Product Information, Product Description). It tokenizes the raw text using Keras Tokenizer, converting them into padded sequences suitable for LSTM input. The target labels are label-encoded and one-hot encoded. The data is split into training and testing sets. The model consists of an embedding layer followed by stacked LSTM layers with dropout for regularization, and dense layers ending in a softmax activation for multiclass classification. After training the model, its performance is evaluated on a test set and the training history (loss and accuracy over epochs) is visualized. 

I have taken the dataset from kaggle, You can access the dataset from [here](https://www.kaggle.com/datasets/PromptCloudHQ/toy-products-on-amazon/data)
