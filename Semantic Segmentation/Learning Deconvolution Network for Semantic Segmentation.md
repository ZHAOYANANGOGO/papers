
# Learning Deconvolution Network for Semantic Segmentation
    Hyeonwoo Noh, Seunghoon Hong, Bohyung Han (ICCV 2015)

本文提出了一个新颖的可学习的语义分割算法，通过使用反卷积网络来识别像素级别的类别标签，并预测分割结果。和之前提出来的FCN模型相比，Deconv模型改进了FCN的两个缺点：  

1. FCN中的receptive field是固定尺寸的，对于输入图片中大的对象，标记的结果可能会产生不一致性，对于输入图片中小的对象可能识别不到。  

2. FCN中反卷积还原的图片结果太粗糙，FCN中的deconvolution结果尺寸为16 X 16，这个尺寸的输出放大到原输入图片尺寸会丢失很多信息。  

![](https://github.com/ZHAOYANANGOGO/papers/blob/master/images/1-1.png)
