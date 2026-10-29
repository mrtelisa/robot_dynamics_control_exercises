# Robot Dynamics and Control: Exercises

Exercises from the lab sessions of the Robot Dynamics and Control course: modelling and control of simple mechanical systems and of 1R and 2R robots in MATLAB/Simulink with **Simscape Multibody**.

> Lab exercises of the Robot Dynamics and Control course (1st year, 2nd semester), MSc Robotics Engineering, University of Genoa. The graded assignments are in [robot_gravity_compensation](https://github.com/mrtelisa/robot_gravity_compensation), [newton_euler_dynamics](https://github.com/mrtelisa/newton_euler_dynamics) and [robot_dynamic_control](https://github.com/mrtelisa/robot_dynamic_control).

## Content

| Session | Exercise | Content |
|---|---|---|
| **1** (`Es1/`) | `es1` | Two-mass spring-mass-damper system, with two PID controllers that bring the masses to the desired positions |
| | `es2` | Base model of a 2R robot, used in the following exercises |
| | `es3_1R`, `es3_2R` | Gravity compensation: a 1R and a 2R robot held still by compensating their weight |
| **2** (`Es2/`) | `es4_OL` | Recursive Newton-Euler algorithm driving the 2R robot in open loop |
| | `es4_CL` | Same, with a PD controller on position and velocity (closed loop) |
| **3** (`Es3/`) | `es5_PD_GC` | PD control with gravity compensation |
| | `es5_CT` | Computed torque control, with three blocks computing the A, B and C matrices of the dynamic model |
| | `es6_NE` | Computed torque control using the Newton-Euler algorithm for the robot dynamics. The result is equivalent to the closed-loop Newton-Euler of `es4_CL` |

Each folder contains the Simulink models, the initialization scripts (`init_robot*.m`, `load_param_and_robot*.m`) and the slides of the session.

## Usage

Requires MATLAB with Simulink and Simscape Multibody. Run the initialization script of an exercise, then open and run its `.slx` model.
