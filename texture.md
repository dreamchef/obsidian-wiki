
#graphics #concept

Add detail without explicit modeling.

# Image map Types
A 2D image is used to texture the surface 
- (takes memory).
- Uses u-v coords
## u-v Coordinate lookup
u, [[basis]] corresponding to $x$-axis.
v corresponds to $y$-axis
1. #todo #q how does uv work?
# Procedural map
Given coordinates, outputs color based on mathematical equations (curves)
- Takes computation time
- Used for natural elements
- Uses location coords**

## Function example
```
Color woodGrain(double x,y,z) {
	double radius = sqrt( (x\*x + z\*z) ) ;
	double angle;
	if (x==0){
		angle = PI/2.0;
	} 
	else {
		angle = arctan(z/x);
	}
	//perturb the radius by an amount based on angle and height 
	radius = radius + (2 \* sin(20\*angle + y/150) ) ;
	//map radius into the range (0..59) 
	double grain = round(radius) % 60 ;
	//choose light grain 2/3 of the time, dark grain 1/3 
	if (grain < 40) {
		return lightColor;
		//e.g. RGB = \[204, 153, 0\]
	} 
	else {
		return darkColor; 
		//e.g. RGB = \[153, 102, 51\]
	}
}
```
