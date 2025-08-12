# Computational-Complexity-
This Java program simulates task scheduling across multiple machines using a greedy algorithm to balance workload and minimize completion time.

It first defines a MachineTaskUpScale class to represent each machine, storing its ID, task description, maximum capacity, and current load. 
The canAssign method checks if a task can be added without exceeding capacity, while assignTask updates the load when a task is assigned.

In the Main class, it creates a list of 12 machines with predefined capacities and descriptions. It then generates 150 random tasks,
each with a duration between 1 and 300 milliseconds. These tasks are sorted in descending order, so larger tasks are assigned first.

The assignment process chooses the least-loaded machine that can still take the task. If no machine has enough remaining capacity, 
the task goes to the least-loaded machine regardless.

Finally, it prints each machine’s total load, the total task time, and the overall completion time in milliseconds and minutes. 
This models a load balancing and scheduling problem often seen in computational complexity and operations research.
