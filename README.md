# *"Next word"* Prediction 

Through the use of natural language processing and deep learning methods, I made a model that is capable of predicting the next word of a particular sentence. From the reading of the text from the book [Metamorphosis](https://www.gutenberg.org/cache/epub/5200/pg5200.txt) by Franz Kafka found in Project Gutenberg, the construction of a deep neural network is used with recurrent neural networks (LSTM). The objective of this project is to have an approach to NLP through Deep Learning.

## Building the model

In the [nxtWordPrediction](https://github.com/yepedraza/nextword-predict/blob/80307bdc413d959ab60544853bc9f9044ca28872/nxtWordPrediction.ipynb) file I carry out the construction of the model, but first I carry out a data preprocessing with the following characteristics:
  * Reading the text with utf8 encoding
  * Use of non-repeating words
  * [Tokenization](https://keras.io/api/preprocessing/text/) of the text for use in the model
  * Sequential model inputs
  * Categorical model outputs

The model architecture is the following:
  * Input Embedding layer
  * Two LSTM layers
  * A fully connected layer and,
  * An output layer

The model has 15,7M training parameters aprox and you can download it [here](https://drive.google.com/file/d/1JX7TPaFdbUDP95Jwxpf5MbWUIis97Oj3/view?usp=sharing)

## Testing the model

For the prediction of the model I created a [notebook](https://github.com/yepedraza/nextword-predict/blob/80307bdc413d959ab60544853bc9f9044ca28872/predScript.ipynb) that has the following characteristics:
  * Model and tokenizer file uploading
  * Use of tokenizer for the input sentences for which we should make the predictions on
  * Make predictions on the input sentence by using the saved model
