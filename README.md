# Reactive Agent

This is an implementation of a simple reactive agent, also known as **Vacuum cleaner** agent.

The agent is placed in a two dimensional space represented by an **array** of **_free cells_**, cells 
containing **_artifacts_** and **_obstacles_**. At each moment the agent can chose randomly between two 
actions: **turn** or **move forward** in the next cell (the movements are restricted by map's border 
and obstacles). The agent does not know whether it can accomplish an action unless it tries. In case the
movement is not possible he **reacts** by turning another way.

Agents objectiv is to collect all artifacts (an artifact is collected once the agents moves in the
cell containing the artifact) and to return to its initial position.

In order to evaluate agent's effiecnecy, the application keeps track of score:
- each action decreases the score by 1 point
- each collected artifact adds 100 points to the score

## Interface 

![demo](https://raw.githubusercontent.com/Iulian-Stan/ReactiveAgent/2742da6dc7aeb271c5d69b61a67cba3303de1c2d/demo.PNG)
