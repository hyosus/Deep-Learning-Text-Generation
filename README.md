# Deep-Learning-Text-Generation
The goal of this assignment is to create an Character Level Text Generation RNN model that predicts the next character given all of the preceding characters in a sequence of data specified by the user using the input() method, resulting in a 400-character paragraph. 

**Approach** <br>
The approach is to create a vocabulary dictionary first, utilising all the unique letters of the corpus's text as keys and the index of each letter starting at zero. It will then be transformed into one-hot vectors and fed as training sequence input characters into the model. The model will then compute the output layer and run it through softmax to obtain the outputs as probabilities. 
