
# CB3 – SignSight : A Robust Deep Vision Framework for Real-Time Perception of Traffic Sign Under Adverse Weather Conditions

## Team Info
- 22471A05H9 — **Nallamothu Vinay** ( [LinkedIn](www.linkedin.com/in/vinay-nallamothu-42901b283) )
_Work Done:  Project Lead; Model Selection, Training, Evaluation, Model Building and overall System Integration, Frontend, Documentation, Deployment.

- 22471A05F4 — **Eerlapti Lakshmaiah** ( [LinkedIn](https://www.linkedin.com/in/eerlapati-lakshmaiah-49897b324?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app) )
_Work Done: Feature Engineering, PPT

- 22471A05L0 — **Yepuri Teja Naga Anil Kumar** ( [LinkedIn](https://www.linkedin.com/in/teja-yepuri-51523534b?utm_source=share_via&utm_content=profile&utm_medium=member_android) )
_Work Done: Performance Analysis, Research Analysis


---

## Abstract
Accurate recognition of traffic signs is a
foundation of contemporary autonomous driving systems, and it is an important 
factor in road safety,
lawful driving, and informed vehicle control. However, developing high
reliability in operational environments is still a significant
challenge. Poor weather conditions, partial occlusion by
other cars or obstacles, and the small appearance of traffic
signs tend to face many challenges and fail to provide
consistent detection. Such issues may reduce system
performance and undermine safety-critical decisions. This
model introduces SignSight, a strong deep learning
framework for real time perception of traffic sign and
recognition framework to address and direct these
challenges through a hybrid deep learning architecture. The
approach combines conventional CNNs with Keras for initial
classification complemented with a YOLOv8 detection
pipeline for accurate spatial localization and real-time
prediction. Compared to state-of-the-art models, SignSight
includes weather-robust preprocessing methods and taps
into small-object detection improvements. Taking cues from
recent research such as YOLO-BS and MASG-Net, our
approach utilizes multiscale feature learning along with
context-aware modules to enhance detection of small sized
and blurred traffic signs. Our unified system reached a
highest classification accuracy of 97.4%, with real-time
performance ensured.

---

## Paper Reference (Inspiration)
👉 **[Paper Title Grounding DINO and distillation-enhanced model for advanced traffic sign detection and classification in autonomous vehicles
 ](https://www.sciencedirect.com/science/article/pii/S2215098625000837)**
Original conference/IEEE paper used as inspiration for the model.

---

## Our Improvement Over Existing Paper
The proposed system improves traditional traffic sign recognition approaches by introducing a more robust and real-time detection framework that performs effectively under challenging environmental conditions such as rain, fog, low lighting, and motion blur. It integrates advanced deep learning models capable of detecting and classifying traffic signs with higher accuracy and faster processing speed. The system enhances recognition reliability by incorporating additional preprocessing techniques and post-processing methods such as optical character recognition and visual enhancement strategies to better interpret sign text and symbols. It also supports real-time monitoring through video and webcam input, making it more practical for intelligent transportation and autonomous driving applications. Overall, the system provides improved accuracy, adaptability, scalability, and usability compared to conventional traffic sign recognition methods.

---

## About the Project


The project develops an intelligent system that automatically detects and recognizes traffic signs from images, videos, or live camera input. It uses deep learning techniques to identify different types of traffic signs and display their meaning in real time. The system is designed to work accurately even in challenging conditions such as poor lighting, bad weather, or complex road environments. This system helps improve road safety by assisting drivers and autonomous vehicles in understanding traffic signs correctly and quickly. It reduces the chances of human error, helps drivers follow traffic rules, and supports advanced driver assistance systems. It can also be used in smart transportation systems and driver training applications. The system first takes input in the form of an image, video, or live camera feed. The input is then processed using image enhancement and preprocessing techniques to improve visibility and quality. The processed data is passed to a trained deep learning model that detects and classifies the traffic signs. Finally, the system produces an output by displaying the detected traffic sign along with its label and highlighting it visually on the image or video frame.
---

## Dataset Used
👉 **[GTSRB - German Traffic Sign Recognition Benchmark](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)**

**Dataset Details:**
The system uses the GTSRB (German Traffic Sign Recognition Benchmark) dataset, which is a widely used and publicly available dataset for traffic sign classification tasks. It contains more than 50,000 images categorized into 43 different traffic sign classes, including warning signs, mandatory signs, and prohibitory signs. The images are collected from real road environments and include variations in lighting conditions, weather, sign sizes, rotations, and background complexity, which helps in training a robust and generalized model.

The dataset is organized into training and testing sets, where the training set contains labeled images grouped into class-wise folders, allowing the model to learn specific features of each traffic sign category. The testing set contains unseen images used to evaluate the model’s performance and accuracy. Each image is provided along with annotation and metadata information such as sign boundaries and class labels, enabling effective supervised learning and model validation. The diversity and large size of the dataset make it suitable for developing high-performance traffic sign detection and recognition systems.

---

## Dependencies Used
Python, TensorFlow, PyTorch, YOLO, OpenCV, NumPy, Pandas, Matplotlib, Seaborn, Tesseract OCR, Google Colab

---

## EDA & Preprocessing
Exploratory Data Analysis (EDA) is performed to understand the dataset structure, class distribution, image variations, and potential data imbalance among traffic sign categories. The dataset is analyzed by visualizing sample images, checking the number of images in each class, and examining variations in lighting, orientation, and background complexity. This helps in identifying challenges such as uneven class distribution and noise in images.

Preprocessing is applied to improve data quality and enhance model performance. Images are resized to a uniform dimension to maintain consistency during training. Data normalization is performed to scale pixel values and improve model convergence. Data augmentation techniques such as rotation, flipping, brightness adjustment, and zooming are used to increase dataset diversity and reduce overfitting. Noise reduction and contrast enhancement techniques are also applied to improve image clarity. These preprocessing steps help the model learn important traffic sign features more effectively and improve overall detection and recognition accuracy.

---

## Model Training Info
The model is trained using a deep learning–based object detection and classification approach to accurately identify traffic signs. The training process uses labeled traffic sign images where each image is associated with a specific class. The dataset is divided into training and validation sets to ensure proper learning and performance monitoring. During training, the model learns to extract important visual features such as shapes, colors, symbols, and text patterns from traffic signs. Data augmentation techniques are applied to improve generalization and prevent overfitting. The training process is performed using GPU acceleration to improve computational efficiency and reduce training time. Key performance metrics such as accuracy, loss, precision, and recall are continuously monitored to evaluate model performance and ensure optimal learning. The trained model is then saved and used for real-time traffic sign detection and recognition.


---

## Model Testing / Evaluation
The trained model is evaluated using a separate test dataset containing unseen traffic sign images to measure its generalization and real-world performance. The evaluation process involves testing the model on multiple input types such as static images, recorded videos, and live webcam feeds to verify its real-time detection capability. Several performance metrics, including accuracy, precision, recall, and loss values, are used to assess the model’s effectiveness. The model achieved high testing accuracy while maintaining low prediction errors, demonstrating strong classification and detection performance. Confusion matrix analysis is also performed to examine class-wise prediction performance and identify any misclassification patterns. The testing results confirm that the model performs reliably across different environmental conditions and input formats, making it suitable for practical intelligent transportation and driver assistance applications.
---

## Results
The developed system achieved strong performance in detecting and recognizing traffic signs across multiple categories. The model obtained an overall classification accuracy of 98.7% on the test dataset, demonstrating high reliability in identifying traffic signs. The system also achieved high precision and recall values of approximately 98.3% precision and 98.1% recall, indicating that the model effectively detects traffic signs while minimizing false predictions. The model showed stable training performance with reduced loss values and consistent validation accuracy throughout training.

---

## Limitations & Future Work
Limitations
The system performance may slightly decrease when traffic signs are heavily occluded, damaged, or extremely blurred.
Detection accuracy can be affected in extremely poor weather conditions such as dense fog or heavy rain.
The model is trained on a specific dataset, which may limit generalization to traffic signs from different countries with varying designs.
Real-time processing may require high computational resources, making deployment challenging on low-power devices.

Future Work
Improve robustness by training the model with more diverse and globally collected traffic sign datasets.
Enhance performance under extreme weather and low-visibility conditions using advanced image enhancement techniques.
Extend the system to support multi-language text recognition for international traffic sign understanding.
Integrate the system with advanced driver assistance and autonomous vehicle navigation systems for improved road safety.

---

## Deployment Info
The system is deployed as a web-based application to make traffic sign detection easily accessible and user-friendly. The backend of the application is developed using Flask, which handles model loading, image/video processing, and prediction generation. The frontend is built using HTML and CSS, providing an interactive interface that allows users to upload images or videos and view detection results in real time. The application integrates the trained deep learning model with the web interface, enabling seamless communication between user inputs and prediction outputs.

The deployment is hosted on the Render cloud platform, which provides reliable hosting, scalability, and easy integration with the Flask backend. The platform allows the system to run continuously and be accessed through a web browser without requiring local setup. This deployment approach ensures that the traffic sign detection system is portable, scalable, and accessible for real-world usage and demonstration purposes.

---
