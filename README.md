# 4 DOF Robotic Arm

This 4 DOF (Degrees of Freedom) Robotic Arm was developed as a project for display at the **Robotic Expo** conducted by the **VIT Chennai Robotics Department**. The project showcases the integration of servos and stepper motors for precise movement control, driven by an **Arduino UNO**.

### Concept and Inspiration
The concept of this project was inspired by the **"DIY Arduino Robot Arm with Smartphone Control"** tutorial by **How To Mechatronics**. The 3D files for the arm were taken directly from the video description, as provided by the creator.

### Features
- **Servo Motors**: Two SG90 and Two MG995 servos are used to control the arm's rotation, including wrist, elbow, and shoulder movements.
- **Stepper Motor**: A **Nema 17** stepper motor is used to control a secondary motion mechanism, operated by an **L298N Motor Driver** for precision movement.
- **Arduino UNO**: The control board for the arm, running a custom code to handle the servo and stepper motor actions.
- **Code Logic**: The movement of the arm is programmed to perform specific sequences with various delays, ensuring smooth transitions between positions.

### Components Used
- **Arduino UNO**
- **SG90 Servo Motors (x2)**
- - **MG995 Servo Motors (x2)**
- **Nema 17 Stepper Motor**
- **L298N Motor Driver** for stepper motor control
- **Jumper Wires, Breadboard**, and other necessary accessories

### Code Workflow
The robotic arm is programmed with the following logic:
- Multiple servos (SG90, MG995) control the rotation and positioning of the arm's joints.
- A stepper motor (Nema 17) is utilized for additional movements in a rotational axis.
- The arm executes a series of pre-programmed movements including picking, placing, and rotating objects based on the code in the loop.

### Code Details
- The code implements a variety of servo movements, including rotation between specific degrees (e.g., `servo1.write(81);` for wrist movement).
- The stepper motor rotates in steps of 40, with defined forward and backward movements.
- Delays between servo actions ensure smooth transitions and avoid jerky motions.
- Movement patterns are hardcoded, and there is an alternating pattern for smoother transitions during repetitive tasks.

### Notes
- The provided code is specific to the project and hardcoded for the arm's designed movements.
- This project does not yet include a smartphone interface for control, but future implementations can add remote control features using Bluetooth or Wi-Fi.

---
