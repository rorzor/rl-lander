# rl-lander
Rocket Lander using Reinforcement Learning Experiment 

# Idea
The plan of this project is an initial foray into using reinforcmenent learning in a practical environment. An environment that goeverns the landing of a rocket will act as the means to train an agent.

# Rules

* The rocket object will have the following key attributes:
  * Position, relative to ground level, which can change only in the up/down direction
  * Velocity. This will be affected by acceleration as normal. Gravitational acceleration is -9.8m/s^2 
  * Thrust, which acts to produce acceleration in the opposite direction to gravity 

* The player (or agent) has the ability to **increase** or **decrease** the thrust at any given time. The amount of thrust available at this stage will be from 0 - 3g
* Each time the game starts, the rocket will have a position randomly set between 500-1000m, and have a downward velocity of between 10-30m/s
* The goal is to land the rocket safely in the least amount of time. Theoretically this is achieved by invoking maximum thrust right up to the moment of landing, initated at a time determined by the rocket's postiion and velocity.
* To land **safely**, the rocket must be travelling less than 1m/s when it hits the ground (position is 0m)    
