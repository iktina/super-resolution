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

<img src="https://i4.imageban.ru/out/2022/09/27/1a143b359dd38eeded52baded9f19e28.png" width="300" />  <img src="https://i6.imageban.ru/out/2022/09/27/081b3bffe874572450e9947183ff8dfa.png" width="300" />  

> Input

<img src="https://i5.imageban.ru/out/2022/09/23/8dd872da33d3d4343e93e6bbb3cdcf11.jpg" width="150" />

> ESRGAN / Real-ESRGAN

<img src="https://i6.imageban.ru/out/2022/09/27/6d7dd669fed935dd8d87d747a00e07e9.png" width="300" />  <img src="https://i7.imageban.ru/out/2022/09/27/0448b68052615e29554cea6bd8872feb.png" width="300" />  

