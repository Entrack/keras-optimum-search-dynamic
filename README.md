This is a repo that contains code demonstrating the **work of DQN agent that searches and follows known-value optimum that is changing it's position in time ** over the field of 20x20 steps  
Enviroment allows agent to move in up-down-left-right directions over the **discrete set of coords on the 2D field** of 20x20 points  
Agent knows the optimum value it needs to find and **learns to stably reach and follow it** from any point in a final time (like **50-60k iterations**)
Methods used:
* step penalty
* idle penalty
* edge-touching penalty
* reward for being in an optimum
* path non-consistency penalty
* feeding last 3 steps actions
* feeding last 3 steps fit functions
* feeding time phase
* 128-96-96-64 relu fully connected
* BoltzmannGumbelQPolicy

Environment is given by potential funcitons and changes the optimum location over time  
Some constants are binded to another in an analytical way  
Code runs with rendering and supports gym interface.
