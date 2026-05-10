# SVG
SVG means Scalable Vector Graphics.

It is a way to draw graphics using Maths and XML.

Instead of storing pixels like png/jpg,
svg stores - lines, circles, paths, curves, text, polygons

# SVG vs Canvas

svg is object based, browser remembers every shape.

we can : 
1. edit shape 
2. animate shape
3. move shape
4. attacj events

good for :
diagrams
mind maps
arrows
flowcharts

Canvas is pixel based . 
after drawing browser forgets objects, blur on zoom 

good for :
games
image processing
painting

# Coordinate System 
top-left corner : (0, 0)
(+ve) x axis ->>>>
(+ve) y axis !!! downward

# rectangle
<rect x="50" y="50" width="200" height="100" fill="white" stroke="black" />

# Polygon 
multiple connected points
<polygon 
    points="
    100,50
    150,150
    50,150
    "
    fill="black"
/>
default svg background is white.

# path
path can draw lines, curves, arcs, shapes.
All in one element.

# Path commands

1. M - move cursor without drawing 
2. L - Draw straight line
3. H - horizonatal
4. V - vertical
5. C → Cubic Bézier Curve
6. Q = Quadratic Bézier Curve [controlX controlY endX endY]
control point

Bezier Curve is a mathematical controlled smooth path.
The curve bends toward special point called control points.

imagine start point, end point, magnet in between 
line bends toward the magnet, that magnet is control point.

Q controlX controlY endX endY

Start point
M 50 100
starts here.

End Point
350 100
curve ends here.

Control Point
200 0
pulls curve upward.

changing control point
more upward bend
Q 200 -100

downward curve
Q 200 200
start ----- control point ----- end

The curve does NOT pass THROUGH the control point.
It bends TOWARD it.

border color : stroke = "black"
thickness : stroke-width = "3"
inner area color : fill = "red" // for only path use fill : none

static svg vs dynamic svg
createElementNS()

http://www.w3.org/2000/svg
this is not internet request

this is a string "an XML namespace identifier"
namespace is basically a category label used by internal browser.