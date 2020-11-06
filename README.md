## CNCGraf7Post
This repository is providing an NC-EASY CAM post processor for Fusion 360, based on the work of Tim Schneider, with extended capabilities:

The NC-EASY post processor gives 2 options to split the g-code into multiple files: either one file for each operation, or a new file every time there is a tool change. This is meant to simplify exporting the code on machines where the tools have to be changed manually.

**This new functionnality has not been tested extensively yet. Use with caution, and check the code before running it on your machine!**

(Note that the CNCGraf7 post is not actually included on this repository)

## Parameters
- *makeSubprograms* : set to *true* to activate multiple output. Default is one file per operation.

 - *groupByTool* : set to true to generate new file every time there is a tool change (only active if *makeSubprograms* is also active).

## Tested 
### 2D
* Adaptive clearing
* Pocket
* Face
* Contour
* Bore
### 3D
* Adaptive clearing
* Pocket clearing
* Parallel
* Contour
* Horizontal
* Scallop
* Spiral
* Morphed spiral
### Drilling
* Drilling - rapid out
* Chip breaking
* Deep drilling
* Break through
* 
### Multi-Axis
### Turning

## Disclaimer

This software is provided **AS IS**, **always** simluate the generated g-code prior use on a real mill!  