# DETR: End-to-End Object Detection with Transformers

# Meta
- theme: 
- author: Nicolas Carion, Francisco Massa, Gabriel Synnaeve, Nicolas Usunier, Alexander Kirillov, and Sergey Zagoruyko
- published at: 2020
- keywords: computer vision

# 1. 연구질문
## 선행 연구의 동향 및 한계
-  modern detectors:
  -  require a specialized library
  -  need to define surrogate regression and classification problems on a large set of proposals, anchors, or window centers
-  Set Prediction
-  Transformers and Parallel Decoding
-  Object detection
  
## 연구 필요성 혹은 차별성
- DETR streamline the training pipeline by viewing object detection as a direct set prediction problem
- The main feature of DETR are the conjunction of the bipartite matching loss and transformers with (non-autoregressive) parallel decoding


# 2. 사용된 이론 및 방법론
## 사용 이론

## 연구 방법

# 3. 논문 핵심
## 연구 핵심
- DETR:  a set-based global loss that forces unique predictions via bipartite matching, and a transformer encoder-decoder architecture
  -  Two ingredients are essential for direct set predictions in detection: (1) a set prediction loss that forces unique matching between predicted and ground truth boxes; (2) an architecture that predicts (in a single pass) a set of objects and
 models their relation

# 4. 결론 및 논점
## 연구 의의 및 한계
