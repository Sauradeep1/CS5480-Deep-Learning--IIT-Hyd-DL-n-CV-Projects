
(CNNs for Colorization) (5 + 2 + 2 = 9 marks) In this problem, we will train a convolutional
neural network for a task known as image colorization. That is, given a greyscale
image, we wish to predict the colour at each pixel. This is a difficult problem for many
reasons, one of which being that it is ill-posed: for a single greyscale image, there can be
multiple, equally valid colourings.
________________________________________________________________________________________
(a) Colorization as Regression: Image colorization can be posed as a regression problem,
where we build a model to predict the RGB intensities at each pixel given the
greyscale input. In this case, the outputs are continuous, and so mean-squared error
can be used to train the model. A set of weights for such a model is included with the
assignment. 
ii. (2 marks)  Comment on how the results (output images,
training loss) change as we increase or decrease the number of epochs, and compare
with the model already provided to you (without your changes).

iii. (1 mark) A color space1 is a choice of mapping of colors into three-dimensional
coordinates. Some colors could be close together in one color space, but further
apart in others. The RGB color space is probably the most familiar to you, but
most state-of-the-art colorization models do not use RGB color space. The model
used in colour regression.ipynb computes squared error in RGB color space.
Why could using the RGB color space be problematic?

iv. (1 mark) Most state-of-the-art colorization models frame colorization as a classification
problem instead of a regression problem. Why? (Hint: what does minimizing
squared error encourage?)
______________________________________________________________________________________________
(b) Colorization as Classification: We will select a subset of 24 colors and frame colorization
as a pixel-wise classification problem, where we label each pixel with one of
24 colors. The 24 colors are selected using k-means clustering over colors, and selecting
cluster centers. This has already been done for you, and cluster centers are provided
in colour/colour kmeans*.npy files. For simplicity, we still measure distance in RGB
space. This is not ideal but reduces the dependencies for this assignment.

(1 mark) Run main training loop of CNN in colourization.ipynb on Colab. This
will train a CNN for a few epochs using the cross-entropy objective. It will generate
some images showing the trained result at the end. How do the results compare to
the previous regression model?
