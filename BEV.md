# 1. Summary
- BEVFormer: learns unified BEV representations with spatiotemporal transformersto support multiple autonomous driving perception tasks
    - aggregating spatial information: design spatial cross-attention that each BEV query extracts the spatial features from the regions of interest across camera views
    - aggregating temporal information: propose temporal self-attention to recurrently fuse the history BEV information.
# 1. Problem and solving
- Problem: The most accurate modern neural networks do not operate in real time and require large number of GPUs for training with a large mini-batch-size.
- Solving: address such problems through creating a CNN that operates in real-time on a conventional GPU, and for which training requires only one conventional GPU.

## 2. 기존 연구
