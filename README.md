# CSS324 Homework Assignment 1

## Task 0

Complete `task-0/members.py` with the names and student IDs of your team members. Each
team is composed of up to two members from either the same or different
sections.

## Task 1

(5 points)

### Problem

You have three bottles with capacities of 8, 5, and 3 liters. The 8-liter bottle
is full, containing 8 liters of water, while the other two bottles are empty.
Your goal is to divide the 8 liters of water evenly, so that the 8-liter bottle
and the 5-liter bottle each contain 4 liters of water.

Assume you cannot add any additional water and that there are no scale markings
on the bottles.

### Search Formulation

 - State: a 3-tuple `(a, b, c)` where `a` is the amount of water in the 8-liter
   bottle, `b` is the amount of water in the 5-liter bottle, and `c` is the
   amount of water in the 3-liter bottle.

 - Initial state: `(8, 0, 0)`

 - Goal test: given a state `(a, b, c)`, check if `a==4` and `b==4`

 - Actions: pour water from one bottle to another bottle. However, you can only
   pour until the source bottle is empty or until the destination bottle is
   full.

 - Step cost: amount of water poured from one bottle to another bottle. For
   example, step cost from `(8, 0, 0)` to `(3, 5, 0)` is `5`.

From the search formulation, complete `task-1/water3.py` so that a Uniform-Cost
Graph search in `task-1/ucgs_water3.py` can be properly conducted.

## Task 2

(5 points)

To conduct an A* search on the eight-puzzle problem, we have designed
a heuristic function `h3` using *the number of tiles out of their target row
plus the number of tiles out of their target column*. Implement the function
`h3` in `task-2/eight_puzzle.py`. This will allow an A* graph search can be
properly conducted using the `h3` heuristic function, as found in
`task-2/asg_eight_puzzle.py`. 

## How submit this homework assignment

 - Create a new github account or use a github account of a team member.

 - Fork this repo into your team's account. 

 - Use `git` to clone the forked repo to your local machine(s). See
   `https://docs.github.com/en/get-started/quickstart` for how to use git and
   github.

 - Update the source files according to the tasks described above.

 - Commit and push the updated files to github.

 - Submit your git repo link in Google Classroom before the deadline. Only one
   representative of the team is required to submit the link.


