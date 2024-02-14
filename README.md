Geometric shapes with JavaScript 🤗 

This sets the width and height of the canvas to 800 pixels each, making it a square canvas.

circle Function:

This function draws circles recursively in a spiral pattern.

Parameters:

radius: The radius of the circle.

distanceFromCentre: The distance of the circle from the center.

angle: The angle at which the circle should be drawn.

Logic:

It calculates the x and y coordinates of the center of the circle based on the given distance from the center and the angle.

It then draws the circle using ctx.arc() method.

It checks if the angle has exceeded 2π (a full circle). If it has, the function returns, terminating the recursion.

Otherwise, it calls itself recursively with an updated angle.

main Function:

This function serves as the main loop for the animation.

Logic:It clears the canvas using ctx.clearRect() to prepare for redrawing.

It calls the circle function to draw the circles.

It increments the divider variable, controlling the spiral density.

It requests the next animation frame using requestAnimationFrame(), which recursively calls main() to create a continuous animation loop.

Finally, it returns an arbitrary value 1.248, which doesn't affect the code.

Execution:

The main() function is called at the end to start the animation loop.
