# Deep Learning - Text Generation
The goal of this assignment is to create an Character Level Text Generation RNN model that predicts the next character given all of the preceding characters in a sequence of data specified by the user using the input() method, resulting in a 400-character paragraph. 

**Approach** <br>
The approach is to create a vocabulary dictionary first, utilising all the unique letters of the corpus's text as keys and the index of each letter starting at zero. It will then be transformed into one-hot vectors and fed as training sequence input characters into the model. The model will then compute the output layer and run it through softmax to obtain the outputs as probabilities. 

### Summary
In general, both models' performances were comparable, with GRU slightly outperforming LSTM. GRU has a higher accuracy with about 6% more than LSTM, as well as a lower loss. It is clear from the first epoch that the LSTM produces repetitive words at a low temperature. With regard to the tenth epoch and beyond, both models become incredibly repetitive. Due to the fact that the model was trained on a story book dataset while the seed input is a random made-up sentence, it is difficult for the model to predict the next character or word.
