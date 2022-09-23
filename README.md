# Image Super Resolution

## Welcome
The service receives an image and uses it as an input for a pre-trained model.

## What’s the point?
The service generates higher resolution images using machine learning methods. The service receives an image in binary format and outputs an image in binary format, which is a higher resolution image than the input one.

This implementation assumes the use of one of two generation models at the user's choice `Real-ESRGAN` and `ESRGAN`. `Real-ESRGAN` is a version of `ESRGAN` for image processing from anime. For this reason, the results of the models are so different

## How does it work?

The user must provide a `path to image` to create images based on this string and `select a model` to generate

The parameter `type` is responsible for choosing the model. If this parameter is active (1), then the model `Real-ESRGAN` will be used, if this parameter is not active (0), then the model `ESRGAN` will be used.

Inputs:

* `metod`: SR_GAN
* `input_data`: 
  * image in binary format
  * binary variable `type` to activate a particular model

## Expected result

> Input

[![imageban](https://i1.imageban.ru/out/2022/09/23/43ee31df2e595bb44b8d7b317638c885.jpg)](https://imageban.ru)

> ESRGAN / Real-ESRGAN

<img src="https://i6.imageban.ru/out/2022/09/23/224ce06bc0866e64c46bb0cbf5b1bb66.png" width="300" />  <img src="https://i7.imageban.ru/out/2022/09/23/80e740b81455ea9df5bfc4feee515d0c.png" width="300" />  

> Input

<img src="https://i5.imageban.ru/out/2022/09/23/8dd872da33d3d4343e93e6bbb3cdcf11.jpg" width="150" />

> ESRGAN / Real-ESRGAN

<img src="https://i7.imageban.ru/out/2022/09/23/d230ec0f3d67c206bf51ad80e25808d7.png" width="300" />  <img src="https://i4.imageban.ru/out/2022/09/23/ea6d0a09af042f37f9cdf1a079228e85.png" width="300" />  