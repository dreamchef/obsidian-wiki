
#graphics 

a way of adding detail without explicit modeling.

With an **image map** texture, a 2D image is used to texture the surface. This uses $(u,v)$ coordinates. This takes up storage.

Alternatively, a **procedural map** outputs color at each coordinate position using a mathematical curve. This takes computation time, but is ideal for natural elements.

The `C++` code below uses a procedural map to texture wood grain using trigonometric curves.
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
