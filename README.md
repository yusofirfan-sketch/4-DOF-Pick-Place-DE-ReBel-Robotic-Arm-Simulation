# Fanuc 4-DOF Robotic Pick-and-Place Simulation

A MATLAB-based robotic simulation of a 4-DOF Industrial Fanuc Robot Arm executing a continuous trajectory picking and sorting operation.

## Project Features
* **Inverse Kinematics (IK) Engine:** Analytical solution utilizing the Law of Cosines to solve joint angles ($\theta_1, \theta_2, \theta_3, \theta_4$) dynamically.
* **Cubic Polynomial Trajectory:** Generates smooth, continuous velocity and acceleration transitions over a 20-second operational cycle.
* **Real-Time 3D Visualization:** Displays live robotic movement along with dynamic workpiece pickup/placement (WP1 in Green, WP2 in Red) and a real-time state logger in the Command Window.

## Workstation Coordinates (mm)
* **Home (Rest):** Initialized at home position
* **Workpiece 1 (WP1):** [-200.0, 20.0, 370.5] -> Sorted to **Rack 2** [-180.0, 70.0, 550.0]
* **Workpiece 2 (WP2):** [-200.0, 250.0, 370.5] -> Sorted to **Rack 15** [180.0, 70.0, 500.0]

## How to Run
1. Open MATLAB (R2020a or later recommended).
2. Download and place `main_simulation.m` in your MATLAB directory.
3. Click **Run** to execute the 3D continuous simulation, plot the joint graphs, and output the tracking table.

<img width="800" height="505" alt="gif" src="https://github.com/user-attachments/assets/8834e710-ae4a-47c8-88fb-4f9eb18562aa" />
