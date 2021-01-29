# deep_learning_of_color_names

Task 1: a neural network to get a RGB color vector from a word

Approach and model:

- Tokenization at word level,
- GloVe pre-trained embeddings with 42B words, trained on Common Crawl and with dimension 300,
- Archictecture: embedding layer, single bidirectional LSTM, two dropout layers, one final dense layer,
- training with mean squared error as loss, adamax as optimizer.

Task 2: a neural network to get a word from a RGB color vector

Approach and model:

- Tokenization at word level of colour names,
- Embedding of colour names with the same GloVe pre-trained embeddings,
- Archictecture: 3 bidirectional LSTM layers and one LSTM layer of increasing size, one dropout layer, one final dense layer,
- Training with cosine similarity as loss and adam optimizer,
- Predicting colour names by looking for the closest vectors in the pre-trained embedding matrix

Deep Learning course final assignment
