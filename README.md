# Image-Classification-using-Caltech-UCSD-Birds-200-Dataset


## Dataset

Using https://www.vision.caltech.edu/datasets/cub_200_2011/ dataset
* Dataset info
  - Number of categories: 200
  - Number of images: 11,788
  - Annotations per image: 15 Part Locations, 312 Binary Attributes, 1 Bounding Box

## Main topics covered in methodology
* Modeling
  - implement a fully connected neural network (multi-layer perceptron):
      * Resize the images to be no larger than 32x32.
      * Use the sequential model API in keras to build your network using dense layers
  -  ResNet-101
      *  Use the pretrained ResNet-101 network available in Keras.
  - Visualization
      * t-SNE  
      * filters learned by each model


## Conclusion
* Using 64 * 64 as image size as a step for handle overfitting from the last step 
* step_1
  - Using ResNet101 pre-trained model when trainable = False (freeze the layers of the model )
  - using flattened layer then adding the output layer with the number of classes and SoftMax as an  activation function 
  
* step_2
  - Using ResNet101 pre-trained model when trainable = False but choose 10 last layers to be unfrozeed 
  - Using a flattened layer then adding the output layer with the number of  classes and SoftMax as an activation function with sparse_categorical_crossentropy for the optimizer 


## contact 
![image](https://user-images.githubusercontent.com/60587913/209285099-911ab4b9-604a-45e5-8c96-ce618df56870.png)https://www.linkedin.com/in/%D9%90%D9%90alaa-elkhashap/
