# CMPSC 310 Activity 15
[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ymop5HUw)

## Deadline: April 12 by 9:50am

## Assignment

 For this activity follow [Neural machine translation with a Transformer and Keras](https://www.tensorflow.org/text/tutorials/transformer).
 
## Data

The data used in the tutorial was the Portuguese-English translation dataset from TensorFlow. This data was pre-processed by tokenizing it. The two text tokenizers used for this project which included the English language tokens and Portuguese language tokens. The data was encoded into tokens in pre-processing which will then be later in the process be decoded back into human-readable text.

## Transformer Compentents

The transformer model puts together all the layers previously created and adds the linear dense layer which will output the token probabilities based on the resulting vectors from each layer location. The architecture of the transformer model process connected sets of tokens through self-attnetion. The process groes from the self-attention layer to layer normalization to the dense layer (final layer).

Parts of the transformer include:

# Self-attention Layer
Both the encoder and decoder in the self-attention layer use attention mechanisms. The input vector in this layer is compared to every other vector in the layer to compute the weights. It is then summed with the other vectors to form the attention weightedd sum value. 

# Feed Forward network and Layer Normalization

In both the encoder and the decoder the feed foward network is made up of two linear layers. There is a ReLU activation in-between the two layers and a dropout layer. The layer normalization is a process that uses mean and stardard distribution to reset the data points inbetween different layers. Normalization is used so that the AI trains faster and is more accurate.

# Final Layer

The final layer is the dense layer from the transformer which will give the output token probabilities. The output of the decoder used previously is the input to the final linear layer.

## Submission

Submit completed Colab notebook showing generated output.
