# Comparative Analysis of PID and Fuzzy Logic Controllers for a 2-DOF Robotic Arm

This repository contains the MATLAB and Simulink implementation of trajectory control for a 2-DOF robotic arm. The project compares a PID controller with a Fuzzy Logic Controller (FLC) in terms of accuracy, response quality, and overall tracking performance. The full project report is included.
<img width="509" height="489" alt="image" src="https://github.com/user-attachments/assets/b5370f99-970e-4570-933d-16f3f6d2bcb4" />

## Project Overview

A 2-DOF planar robotic arm is modeled using forward and inverse kinematics. A circular end-effector trajectory is generated and converted to joint space using inverse kinematics. Both PID and fuzzy controllers are then applied to track the joint trajectories.

The study includes:
- Forward and inverse kinematic modeling  
- Trajectory generation  
- PID controller design and parameter tuning  
- Fuzzy Logic Controller design with membership functions and rule base  
- Simulation and comparison of tracking results  

## System Modeling

The robotic arm is modeled in Simulink.  
(Place your modeling diagram image here)

Forward kinematics determine the end-effector position from joint angles, while inverse kinematics compute the joint angles required for a given trajectory.  
(Place your kinematics illustration here)

## PID Controller

The PID controller receives joint angle references and minimizes the tracking error. Parameters were tuned in MATLAB to improve tracking performance.  
(Insert PID response plot here)

## Fuzzy Logic Controller (FLC)

The FLC is designed using:
- Nine membership functions for the desired angle  
- Three membership functions for the error signal  
- A rule base with nine rules  
- Mamdani inference system  

The controller output regulates joint motion based on linguistic rules rather than fixed gains.  
(Insert membership functions and fuzzy surface image here)
<img width="1289" height="775" alt="image" src="https://github.com/user-attachments/assets/33bdd574-7629-45f8-903a-6058b0d755e3" />

## Simulation Results

Both controllers track the reference trajectory with good accuracy. The FLC shows slightly better performance in the initial motion phase due to its adaptive nature.

PID trajectory result:  
(Insert PID trajectory plot here)

FLC trajectory result:  
(Insert FLC trajectory plot here)

## Repository Contents

- Project report (PDF)  
- README.md  
- License file  
- (Add Simulink models and MATLAB scripts as you upload them)

## How to Run

1. Open MATLAB  
2. Load the Simulink models for PID and FLC  
3. Run the trajectory generator  
4. Compare the responses in the scopes  

Works with MATLAB R2022b and newer.

## Author

Amirhossein Ehsani  
University of Tehran
