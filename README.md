# Densenet-121-from-scratch : 


Introduction to DenseNet :


In a traditional feed-forward Convolutional Neural Network ( E.g VGG-16 ), each convolutional layer except the first one (which takes in the input), receives the output of the previous convolutional layer and produces an output feature map that is then passed on to the next convolutional layer.



![1667141173805](https://user-images.githubusercontent.com/99510125/204150864-f1435d8e-3a83-4ea1-8d84-643374c02912.jpeg)


In a DenseNet architecture, each layer is connected to every other layer, hence the name Densely Connected Convolutional Network. For L layers, there are L(L+1)/2 direct connections. For each layer, the feature maps of all the preceding layers are used as inputs, and its own feature maps are used as input for each subsequent layers.


What is the problem we want to solve?



However, as the number of layers in the CNN increase, i.e. as they get deeper, the 'vanishing gradient' problem arises. This means that as the path for information from the input to the output layers increases, it can cause certain information to 'vanish' or get lost which reduces the ability of the network to train effectively.


For more information visit : https://www.linkedin.com/pulse/densely-connected-convolutional-networks-densenet-ayoub-kirouane
