# Meta
- theme: 
- author:
- published at: 2020
- keywords: computer vision,

# 1. Problem and solving
- Problem: The most accurate modern neural networks do not operate in real time and require large number of GPUs for training with a large mini-batch-size.
- Solving: address such problems through creating a CNN that operates in real-time on a conventional GPU, and for which training requires only one conventional GPU.

## 2. 기존 연구
1. Object detection models
    - a modern detector consists of: 
        1. backbone (pretrained on ImageNet)
        2. neck(some layers between backbone and ehad, and these layers are usually used to collect feature maps from different stages)
        3. head (used to predict classes and bounding boxes of objects)
2. Bag of freebies
    - `Bag of freebies`: Methods that can make the object detector receive better acuuracy **without increasing the inference cost**. They only change the training strategy or only increase the training cost.
        1. **Data augmanetation**
           - some researchers put emphasis on object occlusion issues -> random erase, CutOut can randomly selecte the rectangle region in an image and fill in a random or complementary value of zero
        2. **Semantic distribution bias**
           1. problem1: data imbalance between different classes
               - solution: hard negative example mining or online hard example mining in two-stage object detector
           2. problem2: difficult to express the relationship of the degree of asociation between different categoreis with the one-hot hard representation.
               - solution: label smoothing
        3. **Objective function of Bounding Box (BBox) regression**
           - IoU loss, GIoU loss, CIoU loss
3. Bag of specials
    - `Bag of specials`: plugin modules and post-processing methods that only **increase the inference cost** by a small amount but can significantly improve the acuracy of object detection.(e.g. enlarging receptive field, introducing attention mechanism, or strengthening feature integration capability etc.)
        1. enhanve receptive field: SPP ASPP, RFB
        2. attention module: **1)** channel-wise attention(representative: Squeeze-and-Excitation) and **2)** pointwise attention(representative: Spatical Attention Module)
        3. good activation function: to make the gradient more efficiently propagated, and not to cause too muc extra computational cost.
    - **Since none of above post-processing methods directly refer to the captured image features, post-processing is no longer required in the subsequent development of an anchor-free method.**

## 3. 사용된 이론 및 방법론 (Theories and Methodologies Used)
- used new features: Weighted-Residual-Connections (WRC), Cross-Stage-Partial-connections(CSP),  Cross mini-Batch Normalization(CmBN), Self-adversarial-training(SAT), Mish activation, Mosaic data augmentation, CmBN, DropBlock regularization, and CIoU loss, and combine some of them to achieve state-of-the-art results

## 4. 논문 핵심 (Core of the Paper)
- The basic aim is fast operating speed of neutral network, in production systems and optimization for parallel computations, rather than the low computation volume theoretical indicator (BFLOP)
- 
## 5. 결론 및 논점 (Conclusion and Discussion)
