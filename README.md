# Reading List about Sensor Fusion and Perception Challenges

# Reading List 1
: focused on general advancements in perception and sensor fusion, primarily citing research on multi-sensor fusion, 3D object detection, and some highly-cited techniques

| No. | Check | Article Name | Author | Organization | Published Year | Why it Matters | Key Contributions |
|-----|-------|--------------|--------|--------------|----------------|----------------|-------------------|
| 1   |       | Multi-Sensor Fusion for Autonomous Vehicles Using Deep Learning |  |  |  | This paper focuses on integrating sensor data from LiDAR, radar, and cameras to enhance the accuracy and robustness of object detection in various driving conditions. | Novel deep learning-based fusion techniques that improve detection accuracy under adverse conditions. |
| 2   |       | Real-time LiDAR-Camera Fusion for Object Detection in Autonomous Driving |  |  |  | LiDAR and cameras are the most commonly used sensors in autonomous driving. This paper presents a real-time sensor fusion method that leverages the complementary strengths of both. | A high-performance fusion algorithm designed to improve object detection while reducing latency in real-time systems. |
| 3   |       | Robust Sensor Fusion for Autonomous Driving in Adverse Weather Conditions |  |  |  | Tackles one of the biggest challenges in perception: sensor degradation in bad weather, such as rain, fog, or snow. | Proposes a fusion algorithm that adapts in real-time to sensor failures or degradations, making autonomous vehicles more reliable in extreme conditions. |
| 4   |       | Efficient Sensor Fusion for Perception in Urban Autonomous Driving |  |  |  | Focuses on the unique challenges posed by highly dynamic urban environments, where the vehicle must process and react to large amounts of data in real-time. | Demonstrates an efficient sensor fusion system that improves object tracking and path planning in busy urban scenarios. |
| 5   |       | Multi-Modal Perception for Autonomous Vehicles Using Sensor Fusion Techniques |  |  |  | Discusses how sensor fusion can be applied to leverage multiple modalities (e.g., LiDAR, radar, cameras) to create a more comprehensive understanding of the environment. | Introduces fusion techniques that not only enhance perception but also reduce sensor redundancy, thus cutting costs. |
| 6   |       | A Comprehensive Survey on Sensor Fusion Techniques in Autonomous Driving |  |  |  | This survey covers various sensor fusion methods, comparing traditional approaches and recent advances in AI-driven fusion for autonomous vehicles. | Provides an in-depth overview of the state-of-the-art techniques and future research directions, making it essential for anyone reviewing the field. |

## Reading List 2
: a more focused list that reflects the most current research and innovations in detection and perception

| No. | Check | Article Name | Author | Organization | Published Year | Why it Matters | Key Contributions |
|-----|-------|--------------|--------|--------------|----------------|----------------|-------------------|
| 1   |   ✅    | DETR: End-to-End Object Detection with Transformers (CVPR 2020) |  |  | 2020 | Introduces a transformer-based architecture that directly predicts bounding boxes and object classes without the need for traditional anchors or post-processing. |  |
| 2   |   ⏳    | BEVFormer: Learning Bird’s-Eye-View Representation from Multi-Camera Images (CVPR 2022) |  |  | 2022 | BEVFormer is crucial for tasks like autonomous navigation in dense urban environments, providing top-down perception of the environment. |  |
| 3   |   ⏳    | PV-RCNN: Point-Voxel Feature Set Abstraction for 3D Object Detection (CVPR 2020) |  |  | 2020 | Combines voxel-based and point-based methods for more accurate 3D detection using LiDAR data. |  |
| 4   |   ⏳    | SqueezeSegV3: Spatially-Adaptive Convolution for Efficient Point-Cloud Segmentation (ICRA 2020) |  |  | 2020 | A leading method in 3D point-cloud segmentation, optimized for real-time performance in autonomous vehicles. |  |
| 5   |   ✅    | [YOLOv4: Optimal Speed and Accuracy of Object Detection (CVPR 2020)](https://arxiv.org/abs/2004.10934) |  |  | 2020 | This version of YOLO is optimized for fast object detection in real-time systems, making it particularly suitable for AVs. |  |
| 6   |   ⏳    | Lift-Splat-Shoot: A Lifting Method for 3D Perception Using 2D Images (CVPR 2021) |  |  | 2021 | Converts 2D images to 3D data, useful for creating robust 3D perception models without relying solely on LiDAR. |  |

## Misc_SOTA Tech
| Topic | Overview | Key Methods | Examples |
|-------|----------|-------------|----------|
| Multi-Sensor Fusion | Combines data from LiDAR, radar, cameras, and ultrasonic sensors to improve perception accuracy and robustness. Each sensor compensates for the weaknesses of others. | - Kalman Filters and Particle Filters for probabilistic fusion. <br> - Deep learning-based models like PointPillars and VoxelNet for fusing LiDAR point clouds with camera data. | - VoxelNet: Uses voxelized point cloud data for accurate 3D object detection. <br> - PointPillars: Focuses on fast 3D object detection by creating pillars from LiDAR point clouds. |
| YOLO (You Only Look Once) Object Detection | A real-time object detection algorithm that divides images into grids, predicting bounding boxes and class probabilities. Popular due to its speed and accuracy. | - YOLOv4: Optimized for speed and accuracy, making it useful in real-time AV performance. <br> - YOLOv5 and YOLOv8: Improved hardware efficiency and detection accuracy using advanced architectures like CSPNet. | YOLOv4: Known for its balance of speed and accuracy, crucial in real-time object detection for AVs. |
| 3D Object Detection with Point Clouds | Critical for AVs to understand the environment in 3D, particularly for obstacle detection and navigation. LiDAR-based deep learning methods are state-of-the-art for this task. | - PV-RCNN: Combines point-based and voxel-based methods for efficient 3D detection. <br> - SECOND: A fast, memory-efficient 3D object detection framework using sparse convolutional networks. | - PV-RCNN: Improves both accuracy and efficiency by learning point features with a RoI-based pooling strategy. |
| Deep Learning for Perception and Semantic Segmentation | Helps AVs understand the driving environment by labeling each pixel in an image, detecting roads, lanes, signs, and pedestrians. | - DeepLabv3+: Uses atrous convolution and spatial pyramid pooling for road and lane detection. <br> - UNet: A popular encoder-decoder network used for real-time segmentation. | DeepLabv3+: Widely adopted in AVs for accurate detection of road boundaries, lanes, and traffic signs. |
| Vision Transformers (ViT) for Object Detection | Vision Transformers model global image dependencies effectively, improving the understanding of complex scenes in AVs. | - DETR: Transformer-based object detection framework improving traditional CNN methods, useful for detecting small and occluded objects. <br> - BEVFormer: Uses transformers for bird’s-eye-view perception, helping AVs understand surroundings from a top-down perspective. | DETR: End-to-end object detection approach, faster and more accurate by removing the need for anchors and post-processing. |
| BEV (Bird's Eye View) Perception | Transforms sensor data into a top-down view, offering a holistic understanding of the vehicle’s surroundings. Crucial for lane detection, obstacle avoidance, and trajectory planning. | - BEVFormer: Transformer-based multi-view data processing to enhance accuracy in complex scenarios. <br> - Lift-Splat-Shoot: Lifts 2D images into 3D space, improving AV perception systems. | BEVFormer: Provides AVs with a comprehensive view of surroundings using bird’s-eye-view, effective for urban driving. |
| Adversarial Robustness in Perception Systems | Ensures that AV perception systems are robust against adversarial attacks, such as manipulated images or sensor data that can fool deep learning models. | - Adversarial Training: Uses adversarial examples to make models more robust. <br> - Defensive Distillation: Trains models to reduce sensitivity to small perturbations in input data. | Robust Object Detection: Integrates advanced adversarial defense methods into AV detection pipelines to prevent attacks that could compromise safety. |
