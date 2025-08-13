In this project we train a multi - agent robot to play a simple game against each other using the Reinforcement Learning using PPO gradient.
This is then demonstrted in gazebo simulation using ROS2 humble 
The objective of the game: get a point(shoot the ball outside the back line of the oppponent's court)
Obeservation space: Both agent's positions (x,y) and ball position (x,y,z)
State: Array of current and previous positions of the agents and the ball.
Actions: An agent is able to move in x,y direction. The agent can also move a semicircle part in front of it to punch the ball harder.

Open you terminal and clone:
https://github.com/IsraelAfriyie-dev/Multi-Agent-RL-Simulation.git

Build your work space: 
Colcon build
source install/setup

Run:
ros2 launch robot_gazebo main.launch.xml

Open another terminal and run the training Set:
ros2 run reinforcement_learning ppo_train.py

Training takes about 20hrs to complete, and  after that you can check the log file to see the profile of the training 

