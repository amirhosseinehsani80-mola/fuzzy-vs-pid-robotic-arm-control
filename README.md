# Comparative Analysis of PID and Fuzzy Logic Controllers for a 2-DOF Robotic Arm

This repository contains MATLAB and Simulink files for modeling and controlling a 2-DOF robotic arm. The project compares the performance of a PID controller and a Fuzzy Logic Controller during trajectory tracking. The complete report is included in the repository.
<img width="672" height="561" alt="image" src="https://github.com/user-attachments/assets/6c223ecf-754d-4ad7-bb28-a37599ae83b0" />

## Project Overview

A planar 2-DOF robotic arm is modeled using forward and inverse kinematics. A time-based reference trajectory is generated and converted into joint space through inverse kinematics. Two control methods are then applied to track the joint trajectories. Their accuracy, smoothness, and overall performance are compared.

The project includes:
- Kinematic modeling of the robotic arm  
- Trajectory generation in Cartesian space  
- Conversion of trajectories to joint space  
- PID controller design and tuning  
- Fuzzy Logic Controller design with membership functions and rule base  
- Simulation of both controllers in Simulink  
- Comparison of tracking behavior and control characteristics  

## Modeling Summary

The robotic arm dynamics and kinematics are implemented in Simulink. Forward kinematics determine the end-effector position from joint angles, while inverse kinematics provide the required joint angles for a desired trajectory. These models are used as the basis for both controllers.

## PID Controller

The PID controller uses proportional, integral, and derivative actions to reduce the error between desired and actual joint angles. The gains are tuned using MATLAB tools to achieve stable and accurate tracking. The controller performs well on smooth trajectories and reacts predictably to changes in reference signals.

## Fuzzy Logic Controller

The Fuzzy Logic Controller is designed with membership functions for the desired angle and the tracking error. A Mamdani inference system and a set of nine rules determine the control output. This approach handles the nonlinear behavior of the robotic arm without relying on fixed gains and is more adaptive during transient phases.
<img width="1396" height="752" alt="image" src="https://github.com/user-attachments/assets/4a702272-8dd6-46e0-829f-8b803f110e17" />

## Controller Comparison

Simulations show that both controllers follow the reference trajectory accurately. The PID controller provides a straightforward and effective solution, while the Fuzzy Logic Controller achieves slightly better initial response and smoother adaptation to changes. The FLC demonstrates stronger robustness to nonlinearities and variations in the system.

## Repository Contents

- MATLAB and Simulink files  
- Full project report (PDF)  
- README.md  
- License file  

## How to Use

Open MATLAB, load the Simulink models, and run the simulation files corresponding to the PID and FLC controllers. The results can be compared directly through the scopes and logged data. MATLAB R2022b or newer is recommended.

## Author

Amirhossein Ehsani  
University of Tehran
