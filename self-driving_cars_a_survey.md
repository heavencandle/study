# Summary
- Review and summary about self-driving technology
- Good for grasp technology categories
- Lack of depth and unavailable to tell which technology is SOTA, when to use the method, or what is the strength/weakness of it.

# Lines worth citing
- 
  
# Introduction
- Society of Automotive Engineers (SAE)
- the level of autonomy of a self-driving car: level 0 ~ 5
  - 0: the car's autonomy system issues warnings and may momentarily intervene but has no sustained car control
  - 5: no human intervention is required in any circumstance
- autonomy system of self-driving cars : 1) perception system, 2) decision-making system
  - Perception
    - Localizer
    - Offline Maps
    - Mapper
      - Road Mapping
        
    - MOT
    - TSD
  - Decision Making
    - Route planner
    - Path planner
    - Behavior Selector
    - Motion Planner
    - Obstacle Avoider
    - Controller
# Perception
1. Localization
    - LIDAR-based: motion update, measurement update
        - Normalized Mutual Information, ring compression analysis, leased trimmed squares, Monte Carlo Localization
      - LIDAR plus camera based
      - camera-based: Point Feature based Localization(PFL), Lane Feature based Localization (LFL)
2. Offline and online mapping of unstructured environments
3. Road Mapping
   - Road mapper: responsible for managing information about roads and lanes.
   - Metric Representations
     - grid map: discretizes the environment into a matrix of fixed size cells that contain information about the roads. a wasteful use of memory space and processing time due to buildings, free space, etc
   - Topological Representation
# Decision Making
1. Route Planning
   - Goal directed techniques
   - Separator-based techniques
   - hierarchical techniques
   - bounded-ho techniques
2. Path planning
