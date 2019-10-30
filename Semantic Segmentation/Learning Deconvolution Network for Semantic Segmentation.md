
# Learning Deconvolution Network for Semantic Segmentation
    Hyeonwoo Noh, Seunghoon Hong, Bohyung Han (ICCV 2015)

本文提出了一个新颖的可学习的语义分割算法，通过使用反卷积网络来识别像素级别的类别标签，并预测分割结果。和之前提出来的FCN模型相比，Deconv模型改进了FCN的两个缺点：  

1. 只能接收单一尺寸的语义信息，因为FCN中的receptive field是固定尺寸的，只能解决单尺度语义信息，对于大的对象，标记的结果可能会产生不一致性，对于小的对象识别不到。
2. FCN的deconvolution 产生结果太粗糙，FCN中的deconvolution结果尺寸为16 X 16，这个尺寸的输出通过bilinear interpolation双线性插值放大到输入的图片尺寸，目标中很多信息丢失。
