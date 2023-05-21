# Traffic-Sign-Dectector

The goal of building a CNN-based traffic sign classification system is to improve road safety by increasing the accuracy and reliability of traffic sign recognition. Doing so will help in reducing the chance of accidents caused by human error.

The developed web application provides a user-friendly interface, enabling drivers and traffic authorities to classify traffic signs easily. Real-time feedback enhances decision-making and road safety. This project's outcomes have implications for advanced driver assistance systems, autonomous vehicles, and traffic management, improving performance and safety.

#Processing

A 600mb dataset of more than 50000 images was present. THe images undergo resizing to achieve uniform dimensions,50*50*3 to be exact, facilitating effective model training.

Fine-tune the model by using different kernel sizes and no of filters at each convolution and added some additional layers and batch normalization as well.After every two convolutional layers Max pooling was applied with a stride of 2. Dropouts were used to cater the overfitting problem and ReLu activation function was used to address the vanishing gradients .We then re-trained the model and managed to improve the testing accuracy to 97%.

Trained the new model over the Train folder in the dataset that had 38000+ images with 2.5Million parameters by using the Gpu runtime on Google colab.We had a 75:25 testing to validation split and we ran 20 epochs with the batch size set to 32 which meant that each epoch contained over 981 samples and the learning rate was set to 0.001.We achieved amost 98 percent validation and testing accuracy 

