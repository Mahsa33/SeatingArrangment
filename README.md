# SeatingArrangment

**Problem Description**

The goal of this project is to optimize the seating arrangement for a group of attendees at an event, taking into account potential conflicts between individuals. The problem can be formulated as follows:

**Given**

The number of attendees
The number of rows and columns in the seating arrangement
A conflict matrix that represents the potential conflicts between pairs of attendees
The objective is to find an optimal seating arrangement that minimizes the total number of conflicts among the attendees.

**Solution Approach**

The solution to this problem involves the following steps:

Generate Initial Seating Order: The initial seating order is generated randomly, assigning each attendee to a seat in the seating arrangement.
Analyze Seating Order Conflicts: The function analyze_seating_order_conflicts takes the current seating order and the conflict matrix, and calculates the number of conflicts for each seat in the arrangement.
Update Seating Order: The function update_seating_order identifies the incompatible pairs of attendees (based on the conflict matrix) and swaps the seats of the conflicting attendees to reduce the total number of conflicts.
Iterative Optimization: The process of analyzing the seating order conflicts and updating the seating order is repeated in an iterative manner until a satisfactory solution is found.
Optimization with  MLP: The seating order conflicts are used as input to a MLP model, which is trained to minimize the total number of conflicts. The updated seating order is then used to update the model parameters.
