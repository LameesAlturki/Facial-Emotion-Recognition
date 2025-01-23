## Facial emotion recognition task
The goal of this task is to classify images of human faces into discrete emotional categories based on their facial expressions. This task is challenging due to the subtle and often ambiguous nature of emotional cues in facial expressions. Overall, emotion recognition has the potential to improve interactions across numerous domains, making technology more empathetic and responsive to human needs.

## FER-2013 Dataset
The dataset contains 35,887 labeled facial images categorized into seven emotional expressions: anger, disgust, fear, happiness, sadness, surprise, and neutral divided into training and testing sets.

## Model architecture
This project utilizes a custom implementation of the VGGNet, The variant of VGGnet used is designed to process grayscale images with dimensions (48 x 48 x 1). The network comprises of 4 convolutional stages and 3 fully connected layers. Each of the convolutional stages contains two convolutional blocks and a max pooling layer at the end of each block to reduce spatial dimensions while retaining critical features. The convolution block consists of 3 convolutional layers, with ReLU activation, and a batch normalization layer. The first two fully connected layers are followed by a ReLU activation. The third fully connected layer is for classification.

## Final expirement results
Three experiments with different batch sizes and number of epochs were conducted. The experiment with a batch size 32 and 100 epochs showed the best results with an accuracy of 64%.
