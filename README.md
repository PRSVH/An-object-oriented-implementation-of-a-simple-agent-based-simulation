# An-object-oriented-implementation-of-a-simple-agent-based-simulation
 an agent-based simulation of a simple ecosystem containing three different kinds of organisms: grass, rabbits, and foxes. Agents move over a grid of discrete locations, each containing some grass and at most one animal. Each of these organisms behaves according to a simple set of rules.

Grass grows at every location where an animal is not present.

Rabbits move randomly to empty locations and eat grass.

Foxes move randomly, preferentially moving to neighbouring locations where there are rabbits and eating them.

Animals (both rabbits and foxes) reproduce whenever they are not hungry.

The locations in the world are laid out on a Cartesian grid. Each location has an x and a y coordinate, and eight neighbouring locations, which are those locations with x and y coordinates that differ by no more than 1. The world has periodic boundary conditions, which means that if an animal moves off the right-hand edge of the grid (x == world.sizeX), it reappears on the left-hand edge (x == 0) and vice-versa, and if an animal moves off the bottom edge of the grid (y == world.sizeY), it reappears on the top edge (y == 0) and vice-versa. The boundary conditions are shown for an example 5x4 grid in the diagram below; for example, location 15 has neighbouring locations {14,10,11,19,16,4,0,1}.
The class World.java contains a simple implementation of the simulation.
The GUI visualizes the simulation results.
