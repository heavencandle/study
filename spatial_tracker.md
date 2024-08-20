## Meta
- **Theme**: SpatialTracker: Tracking Any 2D Pixels in 3D Space
- **Author**: Yuxi Xiao, Qianqian Wang, Shangzhan Zhang, Nan Xue, Sida Peng, Yujun Shen, Xiaowei Zhou
- **Published At**: CVPR 2024
- **Keywords**: 2D tracking, 3D space, pixel motion, triplane, occlusion, motion tracking

## 1. 연구질문 (Research Question)
- **Trends and Limitations in Previous Research**: Traditional methods like optical flow and feature tracking struggle with complex 3D motions and occlusions.
- **Necessity or Uniqueness of Research**: This study addresses these challenges by proposing a novel 3D-based tracking method that offers improved accuracy and robustness for long-range pixel tracking, even under occlusion.
- **Research Question**: How can 2D pixels be tracked more effectively by lifting them into 3D space?

## 2. 사용된 이론 및 방법론 (Theories and Methodologies Used)
- **Theories Used**: 3D triplane representation, transformer-based iterative prediction, ARAP (As-Rigid-As-Possible) constraint.
- **Research Method**: The method involves lifting 2D pixels into 3D using monocular depth estimation and employing a transformer-based framework to iteratively predict 3D trajectories.

## 3. 논문 핵심 (Core of the Paper)
- **Core Research**: SpatialTracker introduces a novel framework that tracks pixels in 3D space, leveraging triplane representations and ARAP constraints to improve long-range and occluded pixel tracking performance.

## 4. 결론 및 논점 (Conclusion and Discussion)
- **Research Significance and Limitations**: The method outperforms current state-of-the-art tracking models in several benchmarks, but future improvements could arise from advancements in monocular depth estimation models.






# CVPR_2024_SpatialTracker_Tracking Any 2D Pixels in 3D Space

## Sumary
- Motion estimation's two main paradigms: feature tracking, optical flow
  - optical flow only produces motion for adjacent frames & feature tracking only tracks sparse pixels
- Goal: dense and long-range pixel trajectories in a video
- Proposal: Lift 2D pixels into 3D and perform tracking in the 3D space


## Method
- Given a monocular video as input, our method tracks any given query pixels across the entire video. Different from prior methods that establish correspondences solely
 in the 2D space, we lift pixels to 3D using an off-the shelf monocular depth estimator and perform tracking in a 3D space with richer and more spatially meaningful
 3D contextual information, thereby enhancing the overall tracking performance.

## Key Takeaways
-  a properly designed 3D representation is crucial for solving the long-standing challenge of dense and long-range motion estimation in videos.
