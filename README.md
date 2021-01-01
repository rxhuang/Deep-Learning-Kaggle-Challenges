# Deep-Learning-Kaggle-Challenges

## Challenge 1: https://www.kaggle.com/c/11-785-fall-20-homework-1-part-2
In this challenge you will take your knowledge of feedforward neural networks and apply it to a more useful task than recognizing handwritten digits: speech recognition. You are provided a dataset of audio recordings (utterances) and their phoneme state (subphoneme) labels. The data comes from librispeech that are read aloud and labelled using the original text. 

Solution: Simple feed forward nueral network with Batchnorm and RELU activation.

## Challenge 2: https://www.kaggle.com/c/11-785-fall-20-homework-2-part-2
In this assignment, you will use Convolutional Neural Networks (CNNs) to design an end-to-end system for face verification. Your system will be given two images as input and will output a score that quantifies the similarity between the faces in these images. This helps us decide whether the faces from the two images are of the same person or not.

Solution: CNNs with Batchnorm, Dropout, Maxpool, and RELU activations.

# Challenge 3: https://www.kaggle.com/c/11-785-fall-20-homework-3
Same as challenge 1 but without alignment.
We are going to be using unaligned labels in this contest. That means you are given the list of phonemes for each utterance, but not which frames correspond to which phonemes. Inference of the alignment will require using CTC loss.

Solution: Bidirectional LSTMs with padding.

# Challenge 4: https://www.kaggle.com/c/11-785-fall-20-homework-4-part-2
Same as challenge 3 but without phonemes.

Solution: Pyramidal LSTMs as the encoder. For the decoder, I used individual LSTM cells that takes in attention. Also implemented teacher forcing, gumble noise, and weight tying.  
