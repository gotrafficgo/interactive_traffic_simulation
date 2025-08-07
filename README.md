# Interactive Traffic Simulation

## brief intro
In this (ring-road multi-lane) traffic simulation, one can take the wheel of a car for changing lanes, acceleration and deceleration in real time, also creating congestion. One can observe the traffic dynamics and stop-and-go waves through plotting the time-space diagram of trajectories

## all you need is Matlab
I used R2023a

## how to run the simulation
  0. Make sure everything is under the same folder
  1. Change settings in "Z_Setup.m"
  2. Type "Main_A_Simulation" in Command Window to run the simulation and interactive interface
  3. Type "Main_B_PlotTrajectory" in Command Window to plot the trajectories
  4. Simulation results (data) are saved in the folder "SimulationResult"
Note: I used a MacBook Pro. The position and size of the animation may vary depending on the screen resolution. I will improve it when I have more time.

## how to interact
  1. Press 'Enter' on the keyboard to enter the interactive mode; Press it again to quit
  2. Press 'Up' - Accelerate
  3. Press 'Down' - Decelerate
  4. Press 'Left' - Change lane to left
  5. Press 'Right' - Change lane to right

## model
A variant of Cellular Automata (CA) model is used. see slides for CA https://github.com/gotrafficgo/traffic_flow_theory_slides
  1. Velocity-Dependent-Randomization (VDR) model -- that is why you see two slowdown probabilities in Config.m
  2. Each cell is 1 m long -- that is why you see the animation is quite smooth
  3. Instantanous lane changing

## still working on convincing myself to release all the code
Any suggestions are welcome!

## what does the simulation look like
Video of the simulation and interaction
![Video](demo/video_simulation.gif)

Time-space diagram of trajectoris in a lane
![Diagram](demo/time_space_diagram_of_trajectories_in_one_lane.png)

## Mario version
Try the Super Mario version by downloading "Mario_Version.zip". Have FUN!

![Diagram](demo/Mario.gif)

