# Session10_JahnaviRamagiri

### Objective 1 :
Create a Polygon Class:
where initializer takes in:
number of edges/vertices
circumradius
that can provide these properties:
1. edges
2. vertices
3. interior angle
4. edge length
5. apothem
6. area
7. perimeter

That has these functionalities:
1. a proper __repr__ function
2. implements equality (==) based on # vertices and circumradius (__eq__)
3. implements > based on number of vertices only (__gt__)

### Objective 2:
Implement a Custom Polygon sequence type:
where initializer takes in:
1. number of vertices for largest polygon in the sequence
2. common circumradius for all polygons
That can provide these properties:
1. max efficiency polygon: returns the Polygon with the highest area: perimeter ratio
That has these functionalities:
1. functions as a sequence type (__getitem__)
2. supports the len() function (__len__)
3. has a proper representation (__repr__)

## Regular Polygon
A regular strictly convex polygon is a polygon that has the following characteristics:
all interior angles are less than 180
all sides have equal length 
For a regular strictly convex polygon with:
* n edges (= n vertices)
* R circumradius
* interiorAngle = (n-2)*180/n
* edgeLength,s = 2*R*sin(pi/n)
* apothem,a = R*cos(π/n)
* area = 1/2*n*s*a
* perimeter = n*s

max efficiency polygon = max(area:perimeter ratio)