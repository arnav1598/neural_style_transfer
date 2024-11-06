# Neural Style Transfer

Neural style transfer is an optimization technique used to take three images, a content image, a style reference image (such as an artwork by a famous painter), and the input image (initialized with the content image) you want to style — and blend them together such that the input image is transformed to look like the content image, but “painted” in the style of the style image.

# Visuals

*Content Image*

![](/images/content_image.jpg)

*Style Image*

![](/images/style_image.jpg)

*Output Image*

![](/images/imgb.jpg)

# About

### Objective:
The goal of this project is to implement neural style transfer, a technique that blends the content of one image with the artistic style of another. The final output is a transformed image that retains the content of a content image but is "painted" in the style of a reference style image.

### Approach:

1. Loss Functions:

* Content Loss: Measures the difference in content between the generated image and the content image. It is computed using feature maps from a pretrained convolutional neural network (CNN).
* Style Loss: Measures the difference in style between the generated image and the style image. It involves calculating the Gram matrix of feature maps and comparing them between the generated image and the style reference.

2. Pretrained Model:

Utilized a pretrained CNN model (e.g., VGG19) to extract feature maps for both content and style representations. This model provides a learned representation of various levels of abstraction in images.

3. Optimization:

Employed backpropagation to iteratively update the generated image in order to minimize the combined content and style loss. The optimization process was guided by gradient descent methods, with the Adam optimizer used to adjust the image based on computed gradients.

4. Custom Implementation:

Developed a custom model for handling the optimization process, integrating loss functions and image updates to achieve the desired stylistic transformation.
Outcome: The project successfully demonstrates the ability to transform an input image into a stylized version that reflects the artistic style of a reference image while preserving the content of the original image. The approach effectively balances content and style through iterative optimization, producing visually compelling results.

### References:

[Neural Style Transfer: Creating Art with Deep Learning using tf.keras and eager execution](https://blog.tensorflow.org/2018/08/neural-style-transfer-creating-art-with-deep-learning.html)
