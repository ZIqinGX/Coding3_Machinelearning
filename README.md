# Coding3_Machinelearning

Hi! This is my final project for Coding3 Machine Learning Unit. It is a style transfer exploration example by CNN. My project contains three notebooks. 

## source of dataset:
https://www.kaggle.com/datasets/ikarus777/best-artworks-of-all-time
## code reference:
https://www.tensorflow.org/tutorials/generative/style_transfer#define_content_and_style_representations



## What I did?
The frist notebook is trying to understand how to do style transfer by using two ways: tensorflow Hub and VGG19. I mixed several style pictures with the same content picture. I found that the more unlikely the content picture and the style picture are, the better or obvious mixed style picture can generated. I changed the training steps and feature extactor layers, finding that the training steps and the number of outline layer of VGG can also influence the extend of style mixture. The more training steps, the better mixture effect I can get. So I start to finding more support by trying more times on different pictures in second notebook

The second notebook is trying to further development and try different optimizing way. 

The third notebook is my exploration based on final 1 and final 2 notebook. In this practice, I mainly tried to figure out how the style of content picture will influence the outcome. I found that the content piccture has more color and stronger style and more content, it will remain more details after style transfered, otherwise, the content will be too less to see.

![图片名称](https://github.com/ZIqinGX/CreativeMaking_Advanced_visualisation_and_computational_environment/blob/main/Final%20stage%20video%20shortcut/cover6.png) 

## Findings:
1.From the exploration in the first notebook and second notebook, I found that the greater the difference in style between the content image and the style image, the more pronounced the effect of style transfer.

2.From the third practice in code, I found that the Tensorflow hub model can generate images mainly based on the style. The style image can influence outcome of style transferred picture heavily. By adjusting the weight of content and style picture, the value or influence of them on mixed result will change. So I can adjust pictures by change their weight.

3.Tensorflow Hub is good and fast to do style transfer, however, the style image has a significant impact on the generated image, so it is important to choose content images with strong style and color, or adjust the weight of the style image by multiplying it by a number smaller than 1. VGG model can consume longer time to transfer style and have the problem of noise in image, but it can do more adjustment and the generted content is good.
