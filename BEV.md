# 1. Summary
- BEVFormer: learns unified BEV representations with spatiotemporal transformersto support multiple autonomous driving perception tasks
    - aggregating spatial information: design spatial cross-attention that each BEV query extracts the spatial features from the regions of interest across camera views
    - aggregating temporal information: propose temporal self-attention to recurrently fuse the history BEV information.
# 1. Problem and solving
- Problem
    - **Monocular frameworks & cross-camera post-processing** is most widely used in autonomus driving for visual perception of the surrounding scene to preict the 3D bounding boxes or the semantic maps from 2D cues given by multiple cameras.
        - low performance & efficiency (process different views separately and cannot capture info across cams)
    - BEV is alternative to monocular frameworks.
        - have not shown significant advantages over other paradigm in 3D object detections.
        - a popular BEV generating framework is sensitive to the accuracy of depth values or the depth distributions thus subect to componding errors

- Solving: 

# Summary

## 2. 기존 연구
