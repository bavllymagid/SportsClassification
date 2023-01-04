# Sports Image Classification Report

## Preprocessing :

1. Reading all the training images as RGB
2. Resizing all images to (255,255,3).
3. Split training data into train dataset (80%) and validation dataset
    (20%)
4. Converting training dataset and validation dataset to Batches.
5. Augmenting train dataset.


## Models Description :

### MobileNetV1 Model

**Model Architecture :**


**Training summary :**

using Adam optimizer with learning rate=0.0001 and categorical cross entropy
loss function and early stopping with patience 50 and epochs = 400.

Training accuracy: 0.9940 and validation accuracy: 0.

## Testing accuracy :

- Public test with accuracy 0.
- Private test with accuracy 0.


### VGG19 Model

**Model Architecture :**


**Training summary :**

using Adam optimizer with learning rate=0.0001 and categorical cross entropy
loss function and early stopping with patience 50 and epochs = 400.

Training accuracy: 0.9896 and validation accuracy: 0.

## Testing accuracy :

- Public test with accuracy 0.
- Private test with accuracy 0.


## Conclusion :

MobileNetV1 Model gives best accuracy equals 0.90048 it contains Batch
Normalization layers and depth wise separable layers which improved the
training speed and accuracy.

Depthwise Separable Convolution. This contains two parts.

1. Filtering
2. Combining (combining the 3 color channels to form ’n’ number of
    channels, as desired).

And the Batch Normalization fixes the internal covariate shift issue (In neural
networks, the output of the first layer feeds into the second layer, the output of
the second layer feeds into the third, and soon. When the parameters of a layer
change, so does the distribution of inputs to subsequent layers).


