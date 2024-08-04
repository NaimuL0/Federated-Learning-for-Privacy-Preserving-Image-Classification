# Federated-Learning-for-Privacy-Preserving-Image-Classification

Project Overview
The project focuses on implementing Federated Learning using the TensorFlow Federated (TFF) framework. Federated Learning allows multiple clients (e.g., mobile devices or organizations) to collaboratively learn a shared machine learning model while keeping their training data decentralized. This approach helps in maintaining data privacy and security.

Objective
To create a federated learning model using TFF for classifying handwritten digits from the MNIST dataset.

Dataset: I used the MNIST dataset for simplicity. In practice, this can be replaced with more complex datasets like CIFAR-10, ImageNet, or any proprietary datasets from different institutions.



****This project demonstrates the implementation of a federated learning model using TensorFlow Federated for MNIST digit classification. By distributing the training process across multiple clients, we ensure data privacy and leverage decentralized data for improved model performance.

                          +-------------+
                          |  Central    |
                          |  Server     |
                          +-------------+
                               /|\
                                |
                                |
                        +-------+-------+
                        |       |       |
                   +----+       +----+  ...  +----+
                   |Client 1|  |Client 2|    |Client N|
                   +--------+  +--------+    +--------+

                   
 Visualizations:

 Model: "sequential_8"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d_8 (Conv2D)           (None, 26, 26, 32)        320       
                                                                 
 max_pooling2d_8 (MaxPoolin  (None, 13, 13, 32)        0         
 g2D)                                                            
                                                                 
 flatten_8 (Flatten)         (None, 5408)              0         
                                                                 
 dense_16 (Dense)            (None, 128)               692352    
                                                                 
 dense_17 (Dense)            (None, 10)                1290      
                                                                 
=================================================================
Total params: 693962 (2.65 MB)
Trainable params: 693962 (2.65 MB)
Non-trainable params: 0 (0.00 Byte)
_________________________________________________________________



![image](https://github.com/user-attachments/assets/849216f1-c554-46e9-8b07-df8813ae14e2)


