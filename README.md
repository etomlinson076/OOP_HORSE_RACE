# OOP_HORSE_RACE

mermaid
class diagram
```
class Horse{
    int position
    int index
    int trackLength
    init(int index, int trackLength)
    Horse()
    advance()
    printLane()
    bool isWinner()
}

class Race{
    int NUM_HORSES
    int TRACK_LENGTH
    Horse horses[HORSE_NUM]
    Race()
    advance()
}
```

## Race()
```
int header
  set const static int NUM_HORSES to 5
  set constant int TRACK_LENGTH to 15
in constructor
  go through each horse
  initialize that horse by calling it's init
```
## Race.start()
```
set bool keepGoing to true
while keepGoing:
  advance that horse
  print horse lane
  if that horse wins:
    set keepGoing to false

```

## Horse::Horse()
```
  set position to 0
  set index to 0
  set track_length to 15
```

## Horse::init(int index, int trackLength){
```
  my index = index
  my trackLength = trackLength
  my position = 0
```

## Horse::advance
```
  roll a random 0-1 int called coin
  add coin to position
```
## Horse::printLane
```
 for position from 0 to track length
  if position == my pos:
   print index
  otherwise:
    print "."
  print newline
```

## bool Horse::isWinner
```
bool result = false
if pos >= trackLength
  result = true
  print winning message
return result
```


