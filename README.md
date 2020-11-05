## CNCGraf7Post
This repository is providing an CNCGraf / NC-EASY CAM post processor for Fusion 360.  
It is based on the RS 274D post processor configuration from autodesk.

The NC-EASY post processor gives 2 options to split the machie code into multiple files: either one file for each operation, or one file every time there is a tool change. This is meant to simplify exporting the code on machines where the tools have to be changed manually.

**This new functionnality has not been tested extensively yet. Use with caution, and check the code before running it on your machine!**

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

This software is provided **AS IS**, **always** *simluate the generated g-code prior use on a real mill!*  