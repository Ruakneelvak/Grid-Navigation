# Grid-Navigation
Created various reinforcement learning agents within a custom grid environment to find optimal path.

## Problem Statement
The aim is to develop and compare reinforcement learning agents using Q-learning, Dyna-Q, Dyna-Q+, and Prioritized Sweeping algorithms to find the optimal path in a dynamically generated grid environment. The environment consists of a grid of size N x N, where N is an integer between 2 and 10. One of the tiles is randomly selected as the Start Tile (Green) and another as the Target Tile (Destination - Red). Several other tiles are designated as Blocked Tiles (Black), which the agent cannot traverse. The agent's task is to navigate from the start tile to the target tile using the fewest steps possible while avoiding the blocked tiles. The agent must learn and adapt its strategy based on the chosen reinforcement learning algorithm.

### Algorithms -
1. Q-learning is an off-policy algorithm that learns the value of an action in a particular state based on future rewards. The agent updates its Q-values using the Bellman equation to find the optimal policy.
2. Dyna-Q integrates planning, acting, and learning by using real experiences to update the Q-values and simulated experiences to plan future actions.The agent maintains a model of the environment to generate simulated experiences.
3. Dyna-Q+ extends Dyna-Q by incorporating exploration bonuses to encourage the agent to explore less-visited states. The agent uses these exploration bonuses to balance exploration and exploitation more effectively.
4. Prioritized Sweeping focuses on updating states that are likely to result in significant changes in the value function. The agent prioritizes updates for states that have the highest potential impact on learning.

## Reinforcement Learning
Reinforcement learning is a type of machine learning where an agent learns to make decisions by interacting with an environment. Unlike supervised learning, where the algorithm is trained on labeled data, and unsupervised learning, which deals with unlabeled data, reinforcement learning relies on a feedback mechanism called rewards and penalties.

### Why reinforcement learning
Reinforcement learning is valuable for several reasons:
● Complex Decision-Making: Reinforcement learning is effective for tasks where decisions are complex and involve interacting with dynamic environments. Examples include robot navigation, game playing, and autonomous driving, where decisions depend on real-time feedback and uncertainty.
● Adaptability: Reinforcement learning allows agents to adapt to changing environments and learn optimal strategies over time. This adaptability is crucial in scenarios where conditions may vary, such as in financial markets or resource management.
● Trial and Error Learning: Reinforcement learning enables agents to learn through trial and error, exploring different actions and learning from the outcomes. This iterative learning process is beneficial for tasks with no predefined solution or where exploration is necessary to discover optimal strategies.
● Optimization: The goal of reinforcement learning is to maximize cumulative rewards over time, leading to optimized decision-making. This optimization can lead to cost savings, improved efficiency, and better performance in various applications.
● Dynamic Environments: In environments where the rules or conditions change frequently, reinforcement learning excels. It can adapt to new scenarios, handle uncertainties, and continue learning without the need for explicit programming.

### Evaluation Criteria -

Number of Steps : Measure the number of steps taken by the agent to reach the target tile from the start tile.
Number of Episodes : Assess the number of episodes required for the agent to reach the optimal path.
Stability and Convergence: Evaluate how stable the agent's learning process is and how quickly it converges to an optimal or near-optimal solution.

Agents using different algorithms are expected to exhibit varying performance in terms of Number of steps taken, Number of episodes and Convergence and Stability. A comprehensive comparison of the four algorithms will highlight their strengths and weaknesses in navigating the grid environment.
Identify the most effective reinforcement learning algorithm for the pathfinding task in a grid environment, considering both the quality of the learned path and the computational efficiency of the learning process
