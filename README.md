## Neural Style Transfer

Neural style transfer is an optimization technique used to take three images, a content image, a style reference image (such as an artwork by a famous painter), and the input image (usually same as content image) you want to style — and blend them together such that the input image is transformed to look like the content image, but “painted” in the style of the style image.

## Visuals

Content Image
![Alt text](/images/content_image.jpg)

Style Image
![Alt text]/images/style_image.jpg)

Output Image
![Alt text](/images/imgb.jpg)

## About

* Built several different loss functions and used backpropagation to transform the input image in order to minimize the losses.
* In order to do this, loaded a pretrained model and used its learned feature maps to describe the content and style representation of the images.
* Main loss functions primarily compute the distance in terms of these different representations.
* Implemented this with a custom model.
* Built the custom model with the Functional API.
* Iteratively updated the image by applying the optimizers update rules. 
* The optimizer minimized the given losses with respect to the input image.
