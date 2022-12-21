# Elevator System Algorithm

### This algorithm manages functioning of all elevators in a building.

In the beginning, a user chooses a number of elevators and floors. Doing the next step of the simulation relies on user's reaction by pressing the right key. Then user calls elevators from different floors by specifying a floor number and direction. If a door of a specific elevator opens on a specific floor, user selects all the floors he/she wants to reach. There is information what are the target floors for each elevator. The simulation is on until user decides to stop it.

The main idea of the algoritm is that every elevator works independently. Meaning that an elevator doesn't obtain information about other elevators. Another foundation of the algorithm is distinction whether an elevator is empty or not. The foundation was also assigning a direction attribute to every elevator, which improved the whole logic of the algoritm.

The algoritm takes advantage of FCFS concept (first-come, first-served) in a modified way. If an empty elevator goes for a specific floor which it was called from, it takes other people along the way (when of course the direction of a button is aligned with the direction of an elevator), so the FCFS doesn't apply here. Unless, direction of the empty elevator is opposite to the direction shown by button. So the conclusion is that the FCFS applies to some cases, but not all.
