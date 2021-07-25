# Duelling-DQN-for-ma-gym-Switch

Implementation of Duelling DQN [[1]](#1) to play ma-gym's Switch2-v0 and Switch4-v0 which was done as part of an assignment for my Multi-Agent AI module.

#### Switch2-v0
![Switch-2](https://raw.githubusercontent.com/koulanurag/ma-gym/master/static/gif/Switch2-v0.gif)
#### Switch4-v0
![Switch-4](https://raw.githubusercontent.com/koulanurag/ma-gym/master/static/gif/Switch4-v0.gif)

`Switch-n` is a grid world environment having `n agents` where each agent wants to move their corresponding home location (marked in boxes outlined in same colors).
Each agent receives only it's local position coordinates. The challenging part of the game is to pass through the narrow corridor through which only one agent can pass at a time. They need to coordinate to not block the pathway for the other. A penalty of -0.1 is given to each agent at each timestep, and a reward of +5 for reaching their home cell. The episode ends when all agents have reached their home state or for a maximum of 50 steps in environment.

Action Space: `0: Down, 1: Left, 2: Up , 3: Right, 4: Noop`

Agent Observation : `Agent Coordinate + Steps in env.`


## References
<a id="1">[1]</a> 
Wang, Ziyu, et al. "Dueling network architectures for deep reinforcement learning." International conference on machine learning. PMLR, 2016.
