# CIFAR-10-dataset-Classification using Keras
## Dataset
The CIFAR-10 and CIFAR-100 are labeled subsets of the 80 million tiny images dataset. They were collected by Alex Krizhevsky, Vinod Nair, and Geoffrey Hinton. 
But for this project we will be using the cifar-10 dataset only.

The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.
The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.

Here are the classes in the dataset, as well as 10 random images from each:
<table>
    <tbody><tr>
        <td class="cifar-class-name">airplane</td>
        <td><img src="cifar-10-sample/airplane1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/airplane10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">automobile</td>
        <td><img src="cifar-10-sample/automobile1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/automobile10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">bird</td>
        <td><img src="cifar-10-sample/bird1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/bird10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">cat</td>
        <td><img src="cifar-10-sample/cat1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/cat10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">deer</td>
        <td><img src="cifar-10-sample/deer1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/deer10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">dog</td>
        <td><img src="cifar-10-sample/dog1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/dog10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">frog</td>
        <td><img src="cifar-10-sample/frog1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/frog10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">horse</td>
        <td><img src="cifar-10-sample/horse1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/horse10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">ship</td>
        <td><img src="cifar-10-sample/ship1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/ship10.png" class="cifar-sample"></td>
    </tr>
    <tr>
        <td class="cifar-class-name">truck</td>
        <td><img src="cifar-10-sample/truck1.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck2.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck3.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck4.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck5.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck6.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck7.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck8.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck9.png" class="cifar-sample"></td>
        <td><img src="cifar-10-sample/truck10.png" class="cifar-sample"></td>
    </tr>
</tbody></table>

The classes are completely mutually exclusive. There is no overlap between automobiles and trucks. "Automobile" includes sedans, SUVs, things of that sort. "Truck" includes only big trucks. Neither includes pickup trucks.

## Model Architecture

1. Convolution with 64 filters of size of (3x3)<br>
   Droput layer<br>
   Batch Normalization layer
   
2. Convolution with 128 filters of size of (3x3)<br>
   Droput layer<br>
   Batch Normalization layer
   
3. Convolution with 256 filters of size of (3x3)<br>
   Droput layer<br>
   Batch Normalization layer
   
3. Convolution with 512 filters of size of (3x3)<br>
   Droput layer<br>
   Batch Normalization layer

4. Flatten layer<br>
   Dropout layer<br>

5. Dense layer with 128 neurons<br>
   Dropout layer<br>
   Batch Normalization layer

6. Dense layer with 256 neurons<br>
   Dropout layer<br>
   Batch Normalization layer

7. Dense layer with 512 neurons<br>
   Dropout layer<br>
   Batch Normalization layer

8. Dense layer with 1024 neurons<br>
   Dropout layer<br>
   Batch Normalization layer
   
9. Dense layer with 10 neurons (final layer with softmax activation)<br>


## Implementation accuracy
Train accuracy: 83.69%<br/>
Test accuracy: 83.7%<br/>

We can see that accuracy is not very high. It should be in the range of 95% to 100%. This happened because the model was trained for only 20 epochs. With a bit of tweaking of models layers, number of neurons in the dense layers, dropouts etc and training the model for 100 epochs will result in very high accuracy. But that takes up a lot of resources and time, hence I haven't implemented it for now. You can try it and do tell me what accuracies you get.

## The following additional plots and charts were made to understand the model beter.
<b>Loss vs Epochs</b>

![github-small](plots/cifar10loss.png)


<b>Accuracy vs Epochs</b>

![github-small](plots/cifar10accuracy.png)

<b>Confusion Matrix</b> -- "Truth" stands for the actual value of the classification type whereas "predicted" stands for the predicted classification by the model. 

Here we can see how the confusion matrix  does not have all the elements on the diagonals. This is because of accuracy of 83.7%. As accuracy becomes higher, the diagonal matrix become full whereas rest of the matrix spaces tend to lower numbers. You can go through my <a href="https://github.com/Siddharth-ct/MNIST-dataset-classification-with-TensorFlow">MNIST dataset classification </a> repository to see better confusion matrix results.

![github-small](plots/cifar10cm.png)

<b>Note:</b> Go through the Python Notebook. Each step has been explained briefly.


