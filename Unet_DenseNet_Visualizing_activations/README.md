ASSIGNMENT 3 DL IITH _____________________
PART 1. UNET : Add a skip connection from the first layer to the last, second layer to the second last,
etc. That is, the final convolution should have both the output of the previous layer
and the initial greyscale input as input. This type of skip-connection results in a
“UNet” model.

How does the result compare to the
previous model? Did skip connections improve the validation loss and accuracy? Did
the skip connections improve the output qualitatively? How? Give at least two reasons
why skip connections might improve the performance of our CNN models.

(a) Visualize the activations of the CNN for a few test examples. How are the activation
in the first few layers different from the later layers? You do not need to attach the
output images to your writeup, only descriptions of what you see.
(b) Visualize the activations of the colourization UNet for a few test examples. How do the
activations differ from the CNN activations?
________________________________________________
PART 2 - DENSENET Implementation - 
In DenseNet, each layer obtains additional inputs from all preceding layers and passes on its 
own feature-maps to all subsequent layers. Concatenation is used. Each layer is receiving a “collective knowledge” from all preceding layers.
_________________________________________________
PART 3 - visualizing/understanding CNNs from three perspectives: (i) simple gradient; (ii) Guided backpropagation and (iii) GradCAM.
