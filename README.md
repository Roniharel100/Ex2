Introduction:
This project has two parts.
Part one presents a directed weighted graph.
part two is a pokemon game that uses part one graph methods.

Part one:
The goal of this part is to implement a directional weighted graph.
A directed weighted graph is a graph that has source and destination nodes, and the edges that connect between them. 
in this part we have 6 classes that implemented 6 interfaces:
NodeData implements node_data- represents a single node in a graph. Each node has a unique key, info, tag and location.
GeoLocation implements geo_location- represents the location of the node.
DWGraph_DS implements directed_weighted_graph- This class represent a directed weighted graph.
EdgeData implements edge_data- represents an edge between two nodes in a graph. in this class we can get and set the edges information. 
EdgeLocation implements edge_location- represents the location of the edge.
DWGraph_Algo implement dw_graph_algorithms- in this class we holds a directed weighted graph, and we do actions and algorithms on him.
In addition, we have 3 more classes:
NodeAlgo-we add this class in order to save the father for each node.
Neighbers- we add this class in order to save a hashmap that presents the neighbors of each node.
GraphJson- we add this class in order to save and load the graph in a json format.


Part two:
The goal of this part is to create a pokemon game.
The game is based on the graph that we created in part one.
The game is managed by a server. The server sent information by json format.
 the game has agents and pokemons. the agents need to catch as many pokemon as possible and increase their score. 

game management:
first, we can see that each agent locates near the pokemon that has the highest value.
also each agent is going to the closest pokemon in the graph that no other agent is going after.
We use shortest path algorithm which is in part one, this algorithm helps the agent to know how to go to his closet pokemon.
We have 23 levels in this game. Each level has time till it ends.
To use this game, you need to run the Ex2 class, enter your User ID number and a level number.
In this part we have 5 classes:
Ex2- This class mange and runs the game. This class get from the server id, level number, number of pokemons, number of agents, the time of the game. And after that builds the graph. 
Arena- This class save the game information. This class save the graph, list of pokemons, a list of agents and some function.
Cl_Agent- this class represents an agent in the game.
Cl_Pokemon- this class represents a pokemon in the game.
GameJson- we add this class in order to save the graph in a json format.
 
graphical:
in this part we can see the opening screen.
In this screen you need to enter id and level number between 0 and 23, 
And then the game screen is opening.
In order to show this we made 2 different frames. 
Each frame has a panel. In the panels we draw what we want to show on the screen. 
We also add- timer to count the game time, grade of the level, level number and moves of the level.
In this part we have 3 classes:
GameFrame- Frame is a resizable, movable independent window with a title bar which contains all other components.
In this class we design the frame of the game window.
GamePanel- Panel is an internal region to the frame that helps to group multiple components together.
In this class we design game itself.
Label- In this class we design the opening window of the game.

