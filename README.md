# Vision Based Line Following and Platform Landing for Drones

## Project Aim
Enabled a **Parrot Mambo Minidrone** to autonomously land on a moving platform using **vision-based detection and control**.  
The drone recognized an RGB-colored landing pad mounted on a mobile robot, tracked it in real time, and executed a controlled descent.

---

## Motivation
This project explores coordinated aerial–ground robot systems, which are critical for applications such as:
- Warehouse automation  
- Search and rescue operations  
- Autonomous robotic collaboration in dynamic environments  

---

## Methodology

### System Setup
- Used **MATLAB Simulink** to program the Parrot Mambo drone  
- Mounted a color-coded landing platform on a ground robot  

### Vision & Detection
- **Live Video Stream**: Drone’s onboard camera provided real-time input  
- **Color Segmentation**: MATLAB Color Threshold Tool isolated RGB values of the platform  
- **Frame Partitioning**: Divided camera view into a 3×3 grid (top, bottom, left, right, center)  

### Control & Navigation
- **Directional Movement**: Drone adjusted motion based on zone detection  
  *(e.g., left zone → move left)*  
- **Landing Logic**: Landing triggered only if the platform stayed in the center zone for a set duration  
- **Descent Execution**: Smooth, aligned descent ensured safe landing  

---

## Highlights
- ✅ Reliable Platform Detection: Consistent recognition of the colored platform at low–moderate speeds  
- ✅ Landing Accuracy: Achieved **10–15 cm precision** from the platform center  
- ✅ Motion Coordination: Anticipated robot movement for well-timed descent  

---

## Challenges
- Sensitivity to lighting variations  
- Minor processing delays from onboard computation limits  
- Difficulty in precise end-of-path landings during sudden robot accelerations  

---

## Limitations
- Dependent on stable lighting for color detection  
- Real-time processing bottlenecks caused slight delays  
- Accurate landing at endpoint required better speed estimation  

---

## Future Directions
- Fuse **IMU and GPS data** for improved timing and descent precision  
- Optimize **Simulink models** to reduce processing latency  
- Implement **neural network–based vision systems** for robust detection  
- Explore advanced aerial–ground coordination strategies  

---

## Takeaway
This project demonstrates the integration of **real-time vision, aerial navigation, and ground robot interaction**, showcasing the potential for **autonomous multi-robot collaboration in dynamic environments**.
