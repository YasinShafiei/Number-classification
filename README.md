# Handwritten number classification by Yasin Shafiei

### About this project:
This project will classify handwritten digits using A Convolutional Neural Networks. The model is traiend with the famous `MNIST` dataset.

### Mode:
The CNN model has 1 Convolution and Max-pooling layer, 3 Hidden (Dense) layers and 256 units. 
This is the model summary:
```
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d (Conv2D)             (None, 28, 28, 32)        320       
                                                                 
 max_pooling2d (MaxPooling2D  (None, 14, 14, 32)       0         
 )                                                               
                                                                 
 flatten (Flatten)           (None, 6272)              0         
                                                                 
 dense (Dense)               (None, 256)               1605888   
                                                                 
 dense_1 (Dense)             (None, 256)               65792     
                                                                 
 dropout (Dropout)           (None, 256)               0         
                                                                 
 dense_2 (Dense)             (None, 10)                2570      
                                                                 
=================================================================
Total params: 1,674,570
Trainable params: 1,674,570
Non-trainable params: 0
_________________________________________________________________
```

### Train and Accuracy 
The model accuracy after training for 10 epochs is around 99.71%. 
You can see the model training history as follow:
```
Epoch 1/10
1875/1875 [==============================] - 23s 12ms/step - loss: 0.1818 - accuracy: 0.9445
Epoch 2/10
1875/1875 [==============================] - 22s 12ms/step - loss: 0.0586 - accuracy: 0.9815
Epoch 3/10
1875/1875 [==============================] - 22s 12ms/step - loss: 0.0362 - accuracy: 0.9884
Epoch 4/10
1875/1875 [==============================] - 23s 12ms/step - loss: 0.0244 - accuracy: 0.9918
Epoch 5/10
1875/1875 [==============================] - 22s 12ms/step - loss: 0.0183 - accuracy: 0.9941
Epoch 6/10
1875/1875 [==============================] - 20s 11ms/step - loss: 0.0133 - accuracy: 0.9959
Epoch 7/10
1875/1875 [==============================] - 21s 11ms/step - loss: 0.0124 - accuracy: 0.9957
Epoch 8/10
1875/1875 [==============================] - 21s 11ms/step - loss: 0.0086 - accuracy: 0.9972
Epoch 9/10
1875/1875 [==============================] - 21s 11ms/step - loss: 0.0106 - accuracy: 0.9969
Epoch 10/10
1875/1875 [==============================] - 23s 12ms/step - loss: 0.0086 - accuracy: 0.9971
<keras.callbacks.History at 0x1b8568ca400>
```
### Predictions
THe model test accuracy is around 97 percents. This is the confusion matrix:

![confusion_matrix](https://user-images.githubusercontent.com/91404054/165231051-c7707e73-68b1-4bf1-9e6a-ab475bd0454e.png)


And some of the model predictions:

![2](https://user-images.githubusercontent.com/91404054/165231159-ec5f978e-21ff-4117-994f-1448615c74d4.png)

![3](https://user-images.githubusercontent.com/91404054/165231177-728537f4-4f3a-4db0-9fbc-216aaf6d8eb4.png)

![5](https://user-images.githubusercontent.com/91404054/165231188-a051dc48-3c35-4316-9907-c0e2f75b3670.png)

![6](https://user-images.githubusercontent.com/91404054/165231199-5e4a4af4-0a07-45a1-b562-ade333b49b38.png)

