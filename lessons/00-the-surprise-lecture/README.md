# Lesson 0 - The surprise lecture

## Topics covered

### Image kernels

An image kernel is a small matrix used to apply effects such as blurring, sharpening,
outlining or embossing.

They are used in machine learning for "feature extraction", a technique for determing
the most important portions of the image.

In this context the process is referred generally as "convolution" (as in
[Convolutional Neural Networks](http://setosa.io/ev/image-kernels/)).

#### Kernels

- blur

The blur kernel emphasizes differences in adjacent pixel values.

- emboss

The emboss kernel (similar to the sobel kernel) gives the illusion of depth by
emphasizing the differences in pixels in a given direction.

- identity

The identity kernel leaves the image unchanges.

- outline

The outline kernel is used to highlight large differences in pixel values.

- sharpen

The sharpen kernel emphasizes differences in adjacent pixels values.

- bottom, left, right and top sobel

The sobel kernels are used to show only the differences in adjacent pixel values in
a particular direction.

More information available at [Image Kernels](http://setosa.io/ev/image-kernels/).

### Convolutional Matrix

Convolutional matrix is the treatment of a matrix by another one which is called kernel.

The convolutional matrix filter uses a first matrix which is the image to be treated.
This image is a bi-dimensional collection of pixels rectangular coordinates.

For each pixel, it multiplies the value of the pixel and the values of the 8 surrounding
pixels by the kernel corresponding value. Then it adds the results, and the initial pixel
is set to this final result value.

The filter reads successively, from left to right and top from bottom, all the pixels of
the kernel action area.

More information available at [Convolutional Matrix](https://docs.gikp.org/en/plug-in-convmatrix.html).

### Convolution

It is not a tradicional matrix multiplication, despite being similarly denoted by `*`.

Convolution is the process of adding each element of the image to its local neighbors,
weighted by the kernel.

More information avaliable at [Convolution](https://en.wikipedia.org/wiki/Kernel_(image_processing)#Convolution).

### Sobel operator

The sobel operator is used in image processing and computer vision, particularly within
edge detection algorithms creating an image that emphasizes edges.

More information available at [Sobel Operator](https://en.wikipedia.org/wiki/Sobel_operator).
