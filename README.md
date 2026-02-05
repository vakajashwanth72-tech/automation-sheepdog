# Autonomous Sheepdog – Automation SIG Assignment

## Problem Overview
The objective is to autonomously herd multiple sheep agents into a designated safe zone using a single Sheepdog agent. Sheep exhibit reactive behavior and move away when  sheep dog approached, making direct pursuit ineffective since it can move randomly .

## System Design
The system is designed using ROS 2 concepts such as nodes, topics, and message passing. Each agent operates as a node, and inter-agent communication occurs through published topics but i dont know how to use ros2 so i simply learned thee terminology but did not do practically 

## Herding Strategy
The Sheepdog selects the nearest sheep and positions itself behind it along the line joining the sheep and the safe zone. Since sheep move away from the Sheepdog, this positioning causes the sheep to move toward the safe zone.

## Safe Zone Handling
Sheep that cross the safe zone boundary are despawned and stop publishing their position. The Sheepdog then continues herding remaining sheep.

## Limitations
Due to the development environment being Windows without ROS 2 runtime availability at submission time, the implementation is presented as a complete logical and architectural design using pseudocode.

## Future Scope
- Full ROS 2 implementation and testing
- Improved state-machine based control
- Handling multiple sheep simultaneously

