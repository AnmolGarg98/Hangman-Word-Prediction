## Hangman-Word-Prediction
Predicting a word within six chances of alphabet guessing

Trained LSTM,Bi-LSTM and a Transformer Encoder model with LSTM performing best. 

### Dataset Creation :
Randomly taking a word from the dictionary and padding some alphabets of it. Each alphabet will be 28*1 vector with 26 working as a one-hot representation of A-Z and remaining two for vowel class and whether character is from word or set of wrongly guessed letters. A word will be a matrix of size 38*28 , 32 taken as maximum length of word and 6 for the maximum wrong guessed letters in the game of Hangman. 

Using the above instance of data we will train our sequence model to guess the next possible letter for any random state of the game. On this Random states of data , LSTM performed best with accuracyof 70% which translated to a Win rate of **51.4%** in the whole Hangman Game. 

### Files :
1. train_lstm.ipynb : model training file
2. lstm_exploration_best : model dictionary file 
