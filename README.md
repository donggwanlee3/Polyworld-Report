# PolyWorld: Polygonal Building Extraction with Graph Neural Networks in Satellite Images

## Overview

PolyWorld is an advanced neural network model designed to extract vector representations of buildings from aerial and satellite imagery. The model leverages both Convolutional Neural Networks (CNN) and Graph Neural Networks (GNN) to predict vertices directly and construct precise building polygons. By integrating vertex detection and polygonization into a single process, PolyWorld minimizes error propagation typically seen in multi-stage methods, resulting in superior performance in building extraction tasks.

## Performance

PolyWorld demonstrates notable advancements in the field, outperforming similar models like the FFL approach. Key performance metrics include:

- **Mean Intersection over Union (IoU):** 9.12
- **Combined IoU:** 0.88

These metrics reflect the model's high degree of accuracy in segmenting and delineating building polygons, producing clean and regular polygonal outputs.

### Key Features:

- **End-to-End Process:** Integration of vertex detection and polygonization in a single model.
- **High-Quality Outputs:** The model generates accurate, clean, and regular polygons.

### Figures:

- **Figure 1:** Comparison of Input Image vs Output Results
- **Figure 2:** Additional Visualizations of Model Performance
- **Figure 3:** Edge Case Handling in Output Results

## Limitations

Despite its strengths, PolyWorld has some limitations:

1. **Computational Resources:** The model requires significant computational power and time for training.
2. **Handling Buildings with Holes:** The model struggles with accurately identifying and representing buildings that have internal holes.
3. **Edge Cases:** Buildings that are partially visible at image edges may be inaccurately represented as complete structures.
4. **Multi-Level Structure Discrimination:** The model finds it challenging to distinguish between buildings that are layered on top of each other in complex urban environments.

## Areas for Improvement

To further enhance PolyWorld's capabilities, the following improvements are suggested:

1. **Handling Buildings with Holes:** Implementing additional layers or mechanisms to specifically target the identification and handling of buildings with internal holes.
2. **Edge Case Management:** Training with augmented data that includes edge cases or developing algorithms to infer the continuation of building boundaries beyond the visible area.
3. **Multi-Level Structure Discrimination:** Incorporating elevation data or depth sensors to accurately distinguish between various building levels. Additionally, adapting the model with 3D convolutional networks and enriching training datasets with complex urban scenarios can improve performance in these areas.

## Conclusion

PolyWorld represents a significant advancement in building extraction and polygonization from aerial images, showcasing robust performance and generating high-quality outputs. However, addressing its current limitations and optimizing the training process are crucial for enhancing its practicality and accuracy in real-world applications.
