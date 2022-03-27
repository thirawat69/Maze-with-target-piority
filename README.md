# Maze with target piority

You might be a little confused about the coordinates I'm showing.
Because initially I created the coordinates at (0,0) starting at the top left corner.
But the person who wants to bring my stuff to use, he needs the coordinates (0,0) starting at the bottom left.

In algorithm I implement with A\* algorithm.

So I'm fix the map size and start point in code. Maybe future work I cane dit it.

- map size is 11\*6
- start point (10,3) in coordinates at (0,0) starting at the top left.

## Input

(0,0) starting at the top left

```
lowPiority = [(0,0), (5,4)]
midPiority = [(1,0), (3,2)]
maxPiority = [(1,5)]
wall = [(7,0), (8,0), (9,0), (10,0), (8,1), (9,1), (10,1), (8,4), (9,4), (10,4) ,(7,5) ,(8,5) ,(9,5) ,(10,5)]
```

## Process

```
map, mask = setMap(lowPat, midPat, hardPat, wall)
finalPath = makeFinalPath(map,mask)
```

## Output

(0,0) starting at the top left

```
print(finalPath)
```

```
[[[10, 3], [9, 3], [8, 3], [7, 4], [6, 4], [5, 3], [4, 4], [3, 4], [2, 4], [1, 5]],
 [[2, 4], [2, 3], [2, 2], [2, 1], [1, 0]],
 [[2, 1], [3, 2]],
 [[2, 1], [1, 1], [0, 0]],
 [[1, 1], [2, 2], [3, 3], [4, 3], [5, 4]],
 [[4, 3], [5, 3], [6, 3], [7, 3], [8, 3], [9, 3], [10, 3]]]
```

if (0,0) starting at the bottom left

```
print( patTranform(finalPath) )
```

```
[[[0, 3], [1, 3], [2, 3], [3, 4], [4, 4], [5, 3], [6, 4], [7, 4], [8, 4], [9, 5]],
[[8, 4], [8, 3], [8, 2], [8, 1], [9, 0]],
[[8, 1], [7, 2]],
[[8, 1], [9, 1], [10, 0]],
[[9, 1], [8, 2], [7, 3], [6, 3], [5, 4]],
[[6, 3], [5, 3], [4, 3], [3, 3], [2, 3], [1, 3], [0, 3]]]
```

<img width="1440" alt="Screenshot 2022-03-27" src="https://github.com/thirawat69/Maze-with-target-piority/blob/main/Screenshot%202022-03-27%20.png">
