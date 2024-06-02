# Reinforced Learning Maze

This project is a reinforcement learning implementation for navigating a maze. The agent learns to move within a maze environment, aiming to reach the goal while avoiding obstacles and penalties.

## Description
The agent starts at a specified position in the maze and can perform four actions: move up, move down, move left, and move right. The maze contains various elements, including walls, the goal, and potentially treasure blocks. The agent receives rewards or penalties based on its movements and interactions with these elements.

## Actions and Scenarios
### Actions
+ Up
+ Down
+ Left
+ Right

### Scenarios
1. Moving out of bounds: Action is invalid, agent stays in the same position, penalty of -10.
2. Hitting a wall: Action is invalid, agent stays in the same position, penalty of -10.
3. Reaching the finish point: Action is valid, agent reaches the terminal state, and the process ends.
4. Going back to a previously visited block: Action is valid, but agent receives a penalty of -5 to discourage it from moving back and forth on the same blocks.
5. Moving to a treasure block: Action is valid, agent receives a corresponding reward (Score + 1).
6. Moving to an empty block: Action is valid, agent receives a corresponding reward of 3.