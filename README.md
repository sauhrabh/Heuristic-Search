# Heuristic Search

Project 2 for CPSC 481 summer 2020.

This project continues from [state space search][1].

# Setup

Same as the instructions for [state space search][2].


# Test Functions

+ A* Search:

    `python pacman.py -l tinyMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic`

    `python pacman.py -l mediumMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic`

+ Corners Problem:

    `python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem`

    `python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem`

+ Corners Problem - Heuristic:

    (**NOTE**: Heuristic is consisent because UCS and A* return the same paths (and score) for `tinyCorners` and `mediumCorners`)

    `python pacman.py -l tinyCorners -p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic -z 0.5`

    `python pacman.py -l tinyCorners -p SearchAgent -a fn=uniformCostSearch,prob=CornersProblem,heuristic=cornersHeuristic -z 0.5`

    `python pacman.py -l mediumCorners -p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic -z 0.5`

    `python pacman.py -l mediumCorners -p SearchAgent -a fn=uniformCostSearch,prob=CornersProblem,heuristic=cornersHeuristic -z 0.5`

    Executing the below command expands 978 search nodes:

    `python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5`

+ Eating All the Dots (Food Heuristic)

    `python pacman.py -l testSearch -p SearchAgent -a fn=astar,prob=FoodSearchProblem,heuristic=foodHeuristic`

    Executing the below command expands 4137 search nodes:

    `python pacman.py -l trickySearch -p SearchAgent -a fn=astar,prob=FoodSearchProblem,heuristic=foodHeuristic`

+ Suboptimal Search

    `python pacman.py -l testSearch -p ClosestDotSearchAgent -z 0.5`

    `python pacman.py -l trickySearch -p ClosestDotSearchAgent -z 0.5`
    
    `python pacman.py -l tinySearch -p ClosestDotSearchAgent -z 0.5`
    
    `python pacman.py -l mediumSearch -p ClosestDotSearchAgent -z 0.5`
    
    `python pacman.py -l bigSearch -p ClosestDotSearchAgent -z 0.5`


# Team

| Members                | Email                          | CWID            |
| ---------------------- |:------------------------------:| ---------------:|
| Jacqueline I. Cardenas | jacisac@csu.fullerton.edu      | 889397782       |
| Loai AlFarran          | loayei@csu.fullerton.edu       | 887958254       |
| Saurabh Mishra         | saurabhm2906@csu.fullerton.edu | 887579779       |
| Wayne Lin              | waylin@csu.fullerton.edu       | 887280121       |


[1]: https://github.com/saura8h/State-Space-Search
[2]: https://github.com/saura8h/State-Space-Search#setup
