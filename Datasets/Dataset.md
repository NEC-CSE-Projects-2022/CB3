**📁 Dataset- IP102 Rice Pest Image Dataset (Curated Subset)**
The dataset used in this project is very large, so it is hosted on Google Drive instead of GitHub.

🔗 👉 **[Download Dataset](https://drive.google.com/drive/folders/1OfmkGZ-2pkP_wp_dwrON5mzNlKeK81fN?usp=sharing)**


**📦 Dataset Includes**
  -  Train Dataset – For training the model
  -  Validation Dataset – For tuning the model
  -  Test Dataset – For evaluating performance

**Usage of Dataset**

    The dataset is used to train and evaluate a real-time traffic sign detection and recognition system capable of operating under adverse weather conditions, occlusion, illumination variation, and small-object scenarios. It supports both spatial localization (detection) and fine-grained classification, enabling accurate perception for autonomous driving and intelligent transportation systems


**Dataset Information**

- Dataset Name: German Traffic Sign Recognition Benchmark (GTSRB)
- Source: Public Benchmark Dataset (Stallkamp et al.)
- Domain: Intelligent Transportation Systems / Computer Vision
- Task: Traffic Sign Detection and Multi-Class Classification
- Problem Type: Supervised Learning
- File Format: JPG / PNG images with class labels and bounding boxes
- Dataset Usage: CNN-based classification + YOLOv8-based detection
- Dataset Link: **[Download Dataset](https://drive.google.com/drive/folders/1OfmkGZ-2pkP_wp_dwrON5mzNlKeK81fN?usp=sharing)**


**Dataset Overview**
- Total Records: 50,000+ traffic sign images
- Labeled Records: All images are labeled
- Classes: 43 traffic sign categories
- Annotation Type: Image-level class labels (for CNN classification) Bounding box annotations (for YOLOv8 detection)

In addition to GTSRB, real-world images and video frames containing cluttered backgrounds, vehicles, pedestrians, and multiple signs were used to test robustness in realistic driving environments 




**Why This Dataset?**

This dataset was selected because it provides a realistic and challenging benchmark for traffic sign detection and recognition in real-world driving conditions. Unlike clean or synthetic datasets, it contains traffic signs that are blurred, partially occluded, variably illuminated, and captured at different scales, closely reflecting conditions encountered in autonomous and assisted driving systems. The presence of small, visually similar sign classes forces the model to learn fine-grained discriminative features rather than relying on superficial cues. Its wide acceptance in traffic sign recognition research also enables fair comparison with existing methods, while the availability of both class labels and bounding box annotations supports the development of a unified detection–classification pipeline. These characteristics make the dataset well-suited for evaluating robustness, generalization, and real-time performance of the proposed SignSight framework.


**Features Used**

- Feature 1:Traffic sign shape, color, symbols, and textual patterns
- Feature 2:Spatial and scale-aware features learned through multi-scale detection
- Feature 3: Contextual background cues captured under diverse road conditions


**Summary**

The GTSRB dataset, complemented with real-world traffic imagery, provides a challenging and realistic foundation for developing robust traffic sign perception systems. Its diversity, fine-grained classes, and real-world complexity make it ideal for validating the proposed SignSight framework, which achieves high accuracy and real-time performance under adverse weather and visibility conditions