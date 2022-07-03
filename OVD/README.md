
## Bridging the Gap between Object and Image-level Representations for Open-Vocabulary Detection


  
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;[<sup>1</sup>Hanoona Rasheed](https://scholar.google.com/citations?user=yhDdEuEAAAAJ&hl=en&authuser=1&oi=sra), [<sup>1</sup>Muhammad Maaz](https://scholar.google.com/citations?user=vTy9Te8AAAAJ&hl=en&authuser=1&oi=sra), [<sup>1</sup>Muhammad Uzair Khattak](https://scholar.google.com/citations?user=M6fFL4gAAAAJ&hl=en), [<sup>1,2</sup>Salman Khan](https://salman-h-khan.github.io/), and [<sup>1,3</sup>Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en)



&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; [<sup>1</sup>Mohamed Bin Zayed University of Artificial Intelligene](https://mbzuai.ac.ae/), [<sup>2</sup>Austrailian National University](https://www.anu.edu.au/), [<sup>3</sup>linköping university](https://liu.se/en) 

<br>

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  [Paper](https://arxiv.org/abs/2206.10589): [<img height="25" src="/docs/Paper.PNG" width="25" />](https://arxiv.org/abs/2206.10589)  , [Code:](https://github.com/mmaaz60/EdgeNeXt) [<img height="25" src="/EdgeNeXt/img_1.png" width="25" />](https://github.com/mmaaz60/EdgeNeXt)

<br>

### Abstract

![main figure](images/EdgeNext.png)

In the pursuit of achieving ever-increasing accuracy, large and complex neural networks are usually developed. Such models demand high computational resources and therefore cannot be deployed on edge devices. It is of great interest to build resource-efficient general purpose networks due to their usefulness in several application areas. In this work, we strive to effectively combine the strengths of both CNN and Transformer models and propose a new efficient hybrid architecture EdgeNeXt. Specifically in EdgeNeXt, we introduce split depth-wise transpose attention (SDTA) encoder that splits input tensors into multiple channel groups and utilizes depth-wise convolution along with self-attention across channel dimensions to implicitly increase the receptive field and encode multi-scale features. Our extensive experiments on classification, detection and segmentation tasks, reveal the merits of the proposed approach, outperforming state-of-the-art methods with comparatively lower compute requirements. Our EdgeNeXt model with 1.3M parameters achieves 71.2\% top-1 accuracy on ImageNet-1K, outperforming MobileViT with an absolute gain of 2.2\% with 28\% reduction in FLOPs. Further, our EdgeNeXt model with 5.6M parameters achieves 79.4\% top-1 accuracy on ImageNet-1K.

## Model Zoo

| Name |Acc@1 | #Params | MAdds | Model |
|---|:---:|:---:| :---:|:---:|
| edgenext_small_usi | 81.07 | 5.59M | 1.26G | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.1/edgenext_small_usi.pth)
| edgenext_small | 79.41 | 5.59M | 1.26G | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.0/edgenext_small.pth)
| edgenext_x_small | 74.96 | 2.34M | 538M | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.0/edgenext_x_small.pth)
| edgenext_xx_small | 71.23 | 1.33M | 261M | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.0/edgenext_xx_small.pth)
| edgenext_small_bn_hs | 78.39 | 5.58M | 1.25G | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.0/edgenext_small_bn_hs.pth)
| edgenext_x_small_bn_hs | 74.87 | 2.34M | 536M | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.0/edgenext_x_small_bn_hs.pth)
| edgenext_xx_small_bn_hs | 70.33 | 1.33M | 260M | [model](https://github.com/mmaaz60/EdgeNeXt/releases/download/v1.0/edgenext_xx_small_bn_hs.pth)

### Comparison with SOTA ViTs and Hybrid Architectures
![results](images/madds_vs_top_1.png)

## Comparison with Previous SOTA [MobileViT (ICLR-2022)](https://arxiv.org/abs/2110.02178)
![results](images/table_2.png)

## Qualitative Results (Segmentation)

![results](images/Segmentation.png)

## Qualitative Results (Detection)

![results](images/Detection.png)
