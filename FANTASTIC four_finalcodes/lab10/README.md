# CS362-Lab10

This repository contains the code for Lab-10 of CS362 Course.
It consists of 3 files which are based on the three problems given below.

Suppose that an agent is situated in the 4x3 environment as shown in Figure 1.  Beginning in the start state, it must choose an action at each time step.  The interaction with the environment terminates when the agent reaches one of the goal states, marked +1 or -1.  We assume that the environment is fully observable, so that the agent always knows where it is.  You may decide to take the following four actions in every state:  Up, Down, Left and Right.  However, the environment is stochastic, that means the action that you take may not lead you to the desired state.  Each action achieves the intended effect with probability 0.8, but the rest of the time, the action moves the agent at right angles to the intended direction with equal probabilities.  Furthermore, if the agent bumps into a wall, it stays in the same square.  The immediate reward for moving to any state (s) except for the terminal states S+ is r(s)= -0.04.  And the reward for moving to terminal states is +1 and -1 respectively.  Find the value function corresponding to the optimal policy using value iteration.  

Find the value functions corresponding optimal policy for the following:
r(s)=-2
r(s)=0.1
r(s)=0.02
r(s)=1

[Gbike bicycle rental] You are managing two locations for Gbike.  Each day, some number of customers arrive at each location to rent bicycles.  If you have a bike available, you rent it out and earn INR 10 from Gbike.  If you are out of bikes at that location, then the business is lost.  Bikes become available for renting the day after they are returned.  To help ensure that bicycles are available where they are needed, you can move them between the two locations overnight, at a cost of INR 2 per bike moved.  

Assumptions: Assume that the number of bikes requested and returned at each location are Poisson random variables.  Expected numbers of rental requests are 3 and 4 and returns are 3 and 2 at the first and second locations respectively.  No more than 20 bikes can be parked at either of the locations.  You may move a maximum of 5 bikes from one location to the other in one night.  Consider the discount rate to be 0.9.

Formulate the continuing finite MDP, where time steps are days, the state is the number of bikes at each location at the end of the day, and the actions are the net number of bikes moved between the two locations overnight.

Download and extract files from gbike.zip.  Try to compare your formulation with the code.  Before proceeding further, ensure that you understand the policy iteration clearly.

Write a program for policy iteration and resolve the Gbike bicycle rental problem with the following changes.  One of your employees at the first location rides a bus home each night and lives near the second location.  She is happy to shuttle one bike to the second location for free.  Each additional bike still costs INR 2, as do all bikes moved in the other direction.  In addition, you have limited parking space at each location.  If more than 10 bikes are kept overnight at a location (after any moving of cars), then an additional cost of INR 4 must be incurred to use a second parking lot (independent of how many cars are kept there).  



The reference for the codes:
https://towardsdatascience.com/elucidating-policy-iteration-in-reinforcement-learning-jacks-car-rental-problem-d41b34c8aec7
https://github.com/jainil-4801/cs302
