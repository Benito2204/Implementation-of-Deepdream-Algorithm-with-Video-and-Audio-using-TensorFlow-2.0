# Implementation-of-Deepdream-Algorithm-with-Video-and-Audio-using-TensorFlow-2.0

Deepdream is a Computer Vision algorithm created by Alexander mordvintsev from Google. This algorithm works by creating trippy images.

# How does Deepdream algorithm works?
1. If you feed an image to a CNN, the first layers generally detect low-level features such as edges, circles, etc...
2. As you go deeper in the network, high-level features are then detected such as faces, cars, and trees.

# Let's dive deep into each neurons and see how generate activations
1. When we feed an image into a CNN, the neurons fire and generate activations
2. The deepdream algorithm work by trying to change the input image in a way that would make some of these neurons fire more. we can select any neurons in the layers to make them fire more prominently
3. The process is continuously repeated until the input image now contains all features that a specific layer was originally looking for.

# Deepdream Algorithm Steps:
1. Feed an image into a trained Artificial Neural Network. eg., Inceptionv3
2. Select a layer of choice
3. Calculate the activations
4. Calculate the gradient of the image with respect to the activations of the selected layer
5. Modify the image to increase these activations, and thus enhance the patterns seen by the network resulting in trippy hallucinated image
6. Iterate and repeat over multiple scales

I have used 2 images which consists of mars and eiffel. initially, I blended these 2 images using PIL and feed into the InceptionV3 model.

Here is the link to my colab notebook --> https://colab.research.google.com/drive/1chYR9QLQHPlQM5ufpQvbiGipSyc003ns#scrollTo=sMzXJKv6LMwP.

I would like y'll fork this repository.

Thanks

