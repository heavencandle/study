## Meta
- **Theme**: Conditional Generative Model for Dynamic Trajectory Generation
- **Author**: David Paz, Hengyuan Zhang, Henrik I. Christensen
- **Published At**: University of California, San Diego
- **Keywords**: autonomous driving, navigation, planning, scalable, generative, semantic mapping

## 1. 연구질문 (Research Question)
- **Trends and Limitations in Previous Research**: Existing autonomous driving models either depend heavily on high-definition maps or do not generalize across different vehicles and sensor setups, leading to scalability issues.
- **Necessity or Uniqueness of Research**: The study proposes a novel model, TridentNet, which uses lightweight map representations and conditional generative models to address these issues.
- **Research Question**: How can we generate scalable, vehicle-agnostic trajectories using lightweight representations?

## 2. 사용된 이론 및 방법론 (Theories and Methodologies Used)
- **Theories Used**: Conditional Variational Autoencoder (CVAE)
- **Research Method**: The research employs convolutional layers and a CVAE to generate trajectories using lightweight scene representations and global planning data.

## 3. 논문 핵심 (Core of the Paper)
- **Core Research**: TridentNet dynamically generates ego-centric trajectories without HD maps, leveraging coarse OpenStreetMaps and semantic scene representations.

## 4. 결론 및 논점 (Conclusion and Discussion)
- **Research Significance and Limitations**: The proposed model shows promise with low relative errors, making it feasible for autonomous driving; however, further real-world testing and integration into a hierarchical framework are needed.
