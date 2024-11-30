# Line Follower Robot Project

## Introduction  
This project showcases a simple **Line Follower Robot** that autonomously follows a black line on a contrasting surface. The robot achieves this by using infrared (IR) sensors and basic electronic components, with no microcontroller involved.

---

## Key Features  
- **Autonomous Line Following:** The robot detects and follows a black line without human intervention.  
- **Potentiometer-Controlled Sensor Sensitivity:** Allows fine-tuning of IR sensor thresholds for optimal performance in different lighting and surface conditions.  
- **Minimalist Design:** Simple electronics make it ideal for beginners in robotics and electronics.

---

## Components

### 1. Chassis  
- A sturdy platform that houses the sensors, motors, and power supply.  
- **Material:** Plastic or lightweight metal.

### 2. IR Sensors  
- Two infrared (IR) sensors placed at the front of the robot.  
- **Function:** Detect the contrast between the black line and the surrounding surface, providing input to the motor control system.

### 3. Potentiometer (Sensor Sensitivity Control)  
- **Purpose:**  
  The potentiometer is used to adjust the sensitivity of the IR sensors. This adjustment helps the robot distinguish between subtle variations in surface contrast, ensuring accurate line detection even under varying lighting conditions.

- **Why It's Important:**  
  - Different surfaces reflect light differently, which can affect IR sensor readings.  
  - A surface that is supposed to appear "white" to the sensor may reflect less light under dim lighting, leading to incorrect detection.  
  - By adjusting the potentiometer, the user can set a threshold level where the sensor output changes from detecting a black surface to a white one.  
  - This flexibility allows the robot to operate reliably on different tracks and surfaces, reducing false detections and improving overall performance.

### 4. Motors and Wheels  
- **DC Motors:** Two independent motors control the left and right wheels.  
- **Differential Drive:** The robot steers by adjusting the speed of each motor based on sensor input.  
- **Wheels:** Small rubber wheels provide good traction and smooth movement.

### 5. Power Supply  
- **Battery Pack:** Provides power to the sensors, potentiometer, and motors.  
- **Typical Voltage:** 6V or 9V, depending on motor and sensor specifications.

---

## Working Principle  
1. **Sensor Detection:**  
   The IR sensors continuously monitor the surface beneath the robot.  
   - **Black Surface:** Sensors detect low reflectivity and trigger the appropriate motor control.  
   - **White Surface:** Sensors detect high reflectivity and adjust the motors accordingly.

2. **Potentiometer Adjustment:**  
   The potentiometer allows the user to fine-tune the sensor's sensitivity threshold:  
   - Increase sensitivity to detect faint lines or operate in low light.  
   - Decrease sensitivity to avoid false detection on highly reflective surfaces.

3. **Motor Control:**  
   - **Both sensors detect white:** The robot moves forward.  
   - **Left sensor detects black:** The robot turns left.  
   - **Right sensor detects black:** The robot turns right.  
   - **Both sensors detect black:** The robot may stop or reverse based on circuit design.


## Future Enhancements  
- **Obstacle Avoidance:** Add a simple switch-based or ultrasonic sensor to avoid obstacles.  
- **Speed Control:** Use additional circuitry to allow dynamic speed adjustment.  
- **Multi-Surface Operation:** Incorporate additional sensors to handle complex line-following tasks on uneven or colored surfaces.

