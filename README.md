# Raspberry Pi Cargo Delivery System with Autonomous Drone

Welcome! In our Autonomous Cargo Delivery System project, a drone equipped with technologies such as a Raspberry Pi 4-based mini-computer, OpenCV, and TensorFlow is utilized. Acting as the control unit, the Raspberry Pi 4 manages overall drone control. OpenCV contributes with its image processing capabilities, enabling the drone to understand its surroundings and follow predefined paths. TensorFlow, on the other hand, enhances the drone's learning and adaptation capabilities through deep learning, allowing it to recognize predetermined routes. This technological integration facilitates the drone's autonomous movement and successful completion of tasks. 

![image](https://github.com/eneox/Raspberry-Pi-Cargo-Delivery-System-with-Autonomous-Drone/assets/96574231/aecea30b-1ae0-4d61-abf8-6ef6f6b30225)




## Table of Contents

- [Components](#components)
- [Integration of OpenCV and TensorFlow](#integration-of-opencv-and-tensorflow)
- [How It Works](#how-it-works)
- [PID Controller and Drone Control](#pid-controller-and-drone-control)
- [Enhanced Features](#enhanced-features)
- [Conclusion and Future Developments](#conclusion-and-future-developments)

## Components

1. **Raspberry Pi 4**
   - Main control unit managing overall drone control, data processing, and decision-making processes.

2. **JawsPower 5200 mAh 4S Li-Po**
   - High-capacity power source enabling extended drone operation.

3. **SunnySky X2212-10 980KV**
   - Forward propulsion motors with high torque at low RPM for efficient payload capacity.

4. **FVT LittleBee 20A Dshot 2-4S ESC**
   - Electronic speed controllers regulating motor speed and direction.

5. **MPU6050 6-Axis Accelerometer and Gyro Sensor**
   - Detects drone movement, ensuring stability through accelerometer and gyro data.

6. **GY-NEO6MV2 GPS Module**
   - Determines drone location for navigation towards predefined waypoints.

7. **1045 Drone Propellers**
   - Utilizes power from motors to keep the drone airborne.

8. **Lora E32-433T20D**
   - Enables long-range wireless communication for data transfer and control commands.

9. **Raspberry Pi Camera**
   - Used for imaging and recognizing locations on the map.

10. **Matek FC-HUB Power Distribution Board**
    - Regulates power distribution and supplies power to various components.

## Integration of OpenCV and TensorFlow

The intelligence of the cargo delivery system is driven by the integration of OpenCV and TensorFlow.

### OpenCV (Computer Vision)

- **Lane Detection with OpenCV:**
  - Utilizes color thresholding and edge detection to identify lane markings on the ground for path following.

- **Object Detection:**
  - Employs OpenCV for object detection, enabling the drone to recognize and navigate around obstacles in its path.

### TensorFlow (Neural Networks)

- **Path Recognition:**
  - TensorFlow processes analyzed data, recognizing predefined paths for efficient cargo transport.

- **Adaptive Navigation:**
  - The neural network allows the drone to adapt to changing conditions, making real-time decisions based on visual input from the camera.

## How It Works

1. **Pixel Analysis with OpenCV:**
   - OpenCV performs pixel analysis on images captured by the Raspberry Pi Camera, identifying key features like lane markings and obstacles.

2. **Neural Network Decision-Making with TensorFlow:**
   - TensorFlow processes analyzed data, enabling the drone to recognize predefined paths and make decisions on navigation.

3. **Route Planning:**
   - OpenCV and TensorFlow together enable the drone to determine its route by recognizing familiar paths from the training dataset, facilitating autonomous navigation.

## PID Controller and Drone Control

The PID controller ensures precise control and stability during flight through the Proportional, Integral, and Derivative terms.

- **Proportional (P) Term:**
  - Measures the error between the current state and the target state of the drone, adjusting the drone's position based on this error.

- **Integral (I) Term:**
  - Takes into account the cumulative sum of past errors, eliminating long-term steady-state error.

- **Derivative (D) Term:**
  - Predicts future errors by considering the rate of change, ensuring stability and preventing overshooting.

## Enhanced Features

### Smart Waypoint Navigation

- **GPS-Aided Navigation:**
  - Broadens awareness for long-distance deliveries, facilitating route planning based on global positioning.

- **IMU for Stability:**
  - Utilizes MPU6050 IMU for precise control, ensuring stable and balanced flight.

### Dynamic Obstacle Avoidance

- **Ultrasonic Sensors:**
  - Provide distance measurements to nearby objects.
  - Combined with OpenCV for dynamic obstacle avoidance.

- **Dynamic Path Replanning:**
  - Triggers route adjustments based on detected obstacles.

### Real-Time Communication and Monitoring

- **Telemetry Data:**
  - Sends real-time data (GPS, battery status) to the ground station.
  - Enables constant monitoring of drone health and performance.

# Conclusion and Future Developments

## Conclusion

In conclusion, this Autonomous Cargo Delivery System marks a significant stride in the field of drone technology. The integration of sophisticated hardware components with state-of-the-art computer vision and neural network algorithms empowers the drone with autonomy and adaptability, making it suitable for a wide range of cargo delivery scenarios.

The PID controller ensures precise control and stability, laying the foundation for reliable and efficient flight operations. The smart integration of OpenCV and TensorFlow not only enables the drone to navigate predefined paths but also equips it with the capability to adapt to dynamically changing environments.

## Future Developments

As technology evolves, there are several avenues for future developments and enhancements:

- **Machine Learning Refinement:**
  Continuous training of the neural network with more diverse datasets can further improve the system's ability to recognize and adapt to complex scenarios.

- **Advanced Obstacle Avoidance:**
  Integration of more advanced obstacle avoidance techniques, such as LiDAR sensors, could enhance the drone's ability to navigate through challenging environments with higher precision.

- **Real-Time Decision-Making:**
  Implementing real-time decision-making algorithms can further reduce response times and improve the overall efficiency of the cargo delivery system.

- **Cloud Integration:**
  Exploring the integration of cloud-based services for data storage, analysis, and remote monitoring can open up possibilities for scalability and enhanced analytics.

