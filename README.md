# Geodesic_Distance_Transform
Python module for computation of the geodesic distance transform of an array from a given starting point (array containing distances of each point in the image to the starting point selected)

------------------------------------------------------------------------

Module for computation of chamfer distance transform of an image from a starting point
Default method considers periodic boundaries

Use: gdt.dist(array_input, seed, dist_type)
Where:
	- array_input: numpy binary array representing image (1 - foreground; 0 - background)
	- seed: tuple ((z), y, x) representing coordinates used as starting point for transformation
	- dist_type: distance metric used
		"city" = cityblock
		"chess" = chessboard
		"borges" = borgefors
		"quasi" = quasi-euclidean

Output: array where values represent distance (may be infinite)

----------------------------

Other functions from this module (see corresponding docstrings):
	gdt.form3d(): quick import of 3D images into required format
	gdt.optim(): used for restricting computation to the minimum region containing a list of points

For more information see docstrings for each function
