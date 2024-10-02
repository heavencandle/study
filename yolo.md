# Meta
- theme: 
- author:
- published at: 2020
- keywords: computer vision,

# Problem and solving
- Problem: The most accurate modern neural networks do not operate in real time and require large number of GPUs for training with a large mini-batch-size.
- Solving: address such problems through creating a CNN that operates in real-time on a conventional GPU, and for which training requires only one conventional GPU.

## 1. 연구질문 (Research Question)
- 

## 2. 기존 연구
1. Object detection models
    - a modern detector
        1. backbone (pretrained on ImageNet)
        2. neck(some layers between backbone and ehad, and these layers are usually used to collect feature maps from different stages)
        3. head (used to predict classes and bounding boxes of objects)
2. Bag of freebies
    - `Bag of freebies`: Methods that can make the object detector receive better acuuracy **without increasing the inference cost**. They only change the training strategy or only icnrease the training cost.
        1. Data augmanetation
        2. Semanitc distribution bias
3. Bag of specials
    - `Bag of specials`: plugin modules and post-processing methods that only **increase the inference cost** by a small amount but can significantly improve the acuracy of object detection.

## 3. 사용된 이론 및 방법론 (Theories and Methodologies Used)
- used new features: Weighted-Residual-Connections (WRC), Cross-Stage-Partial-connections(CSP),  Cross mini-Batch Normalization(CmBN), Self-adversarial-training(SAT), Mish activation, Mosaic data augmentation, CmBN, DropBlock regularization, and CIoU loss, and combine some of them to achieve state-of-the-art results

## 4. 논문 핵심 (Core of the Paper)
- The basic aim is fast operating speed of neutral network, in production systems and optimization for parallel computations, rather than the low computation volume theoretical indicator (BFLOP)
- 
## 5. 결론 및 논점 (Conclusion and Discussion)
