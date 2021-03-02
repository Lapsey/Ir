# Drune Rugland Infrared Boe-Bot Script
Simple infrared boe-bot maze navigation script

## Maze Solution Ideas
1. Side pointing IR sensors
2. forward pointing IRs
3. 45deg angled ir sensors

### Side pointing IR sensors
#### Pros
1. easy turn detection
2. very easy implementation

#### Cons 
1. unclear correction detection solution making it very unreliable 
2. sideward facing irs can be physically finicky
3. unclear if with no corrections the maze can be finished 

### Forward facing IR sensors
#### Pros
1. very easy turn detection
2. Stupidly easy implementation

#### Cons 
1. super hard correction detection solution
2. unclear if with no corrections the maze can be finished

### Angled facing
#### Pros
1. reliable side wall detection 
2. easy turn detection 
3. possible correction detection

#### Cons
1. physically finicky 

# Angled solution
1. check the sensors 
2. if both see wall then go forward
3. otherwise
 * correct into the side that doesn't see and adjust the values so the turn works well

## TODO
* [x] Add IR check routine
* [x] Test IR On start up
* [x] Add movement subs
* [x] Figure out a solution to the maze
    * [ ] Forward facing 
    * [ ] sideward facing
    * [x] angled facing 
* [ ] Implement the solution
* [ ] Remove unecessary code 