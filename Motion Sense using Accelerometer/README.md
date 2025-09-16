# MotionSense: Real-Time Movement Classification Using TinyML and Smartphone Accelerometer

##  Overview
MotionSense is a lightweight machine learning project built using Edge Impulse that detects and classifies human movements—specifically **standing**, **rotating**, and **shaking**—using real-time data from a smartphone's built-in accelerometer. This project demonstrates how TinyML can be deployed on edge devices to perform motion classification efficiently without cloud dependency.

##  What is TinyML?
TinyML refers to machine learning models optimized to run on resource-constrained devices like microcontrollers. These models are small, fast, and energy-efficient, making them ideal for real-time applications like motion detection.

##  Hardware Used
- **Smartphone** (used as the 3-axis accelerometer sensor via Edge Impulse mobile app)
- No external microcontroller required for data collection

##  Software & Tools
- [Edge Impulse Studio](https://www.edgeimpulse.com/)
- Edge Impulse Mobile App (for data collection)
- Edge Impulse CLI (for deployment)

##  Project Goals
- Capture real-time motion data from the phone’s accelerometer
- Train a TinyML model to classify three types of motion:
  - **Stand**
  - **Rotate**
  - **Shake**
- Deploy and test the model on-device using Edge Impulse

##  Data Collection
1. Open the Edge Impulse mobile app and connect to your project.
2. Record motion data for each class:
   - **Stand**: Hold the phone still.
   - **Rotate**: Slowly rotate the phone in different directions.
   - **Shake**: Shake the phone vigorously.
3. Collect at least 5–10 minutes of data per class for better accuracy.

##  Model Training
- Use Edge Impulse Studio to:
  - Create impulse (signal processing + learning block)
  - Preprocess accelerometer data
  - Train a classification model (e.g., Decision Tree or Neural Network)
  - Validate model performance using test data

##  Deployment
- Test the model directly on your smartphone using the Edge Impulse app.
- Optionally, export the model to run on microcontrollers (e.g., Arduino, STM32) if needed.

##  Results
- The model achieves high accuracy in distinguishing between the three motion types.
- Real-time inference is fast and efficient on mobile devices.

##  Learnings
- TinyML enables powerful edge intelligence with minimal hardware.
- Smartphones can serve as versatile sensors for prototyping ML applications.
- Edge Impulse simplifies the end-to-end ML workflow for embedded systems.

##  Future Enhancements
- Add more motion classes (e.g., jump, walk, fall)
- Deploy on wearable devices or IoT platforms
- Integrate with alert systems or fitness trackers

##  License
This project is open-source under the MIT License.

##  Acknowledgments
Thanks to Edge Impulse for providing an intuitive platform for embedded ML development.

