## Task
Classify images of human faces into discrete emotional categories based on their facial expressions. This task is challenging due to the subtle and often ambiguous nature of emotional cues in facial expressions.

## FER-2013 Dataset
The dataset contains 35,887 labeled facial images categorized into seven emotional expressions: anger, disgust, fear, happiness, sadness, surprise, and neutral.

## Model architecture
We utilized a custom implementation of the VGGNet, the variant of VGGnet used is designed to process grayscale images with dimensions (48 x 48 x 1). The network comprises of 4 convolutional stages and 3 fully connected layers. Each of the convolutional stages contains two convolutional blocks and a max pooling layer at the end of each block to reduce spatial dimensions while retaining critical features. The convolution block consists of 3 convolutional layers, with ReLU activation, and a batch normalization layer. The first two fully connected layers are followed by a ReLU activation. The third fully connected layer is for classification.

## Results
<img width="840" height="406" alt="image" src="https://github.com/user-attachments/assets/1bbca171-179e-4923-830e-a622b8f0ec23" />

The experiment with a batch size 32 and 100 epochs showed the best results with an accuracy of 64% and the following confusion matrix:

<img width="804" height="701" alt="image" src="https://github.com/user-attachments/assets/9f0e8ee0-bd05-4fa1-84f5-af5b5ee0837a" />

**Full report:** [CSC462-FER-project report.pdf](CSC462-FER-project%20report.pdf)
