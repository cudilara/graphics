# graphics
This repo is for Computer Graphics assignments.

## Homework 2: Lorenz Attractor
Write a three dimensional OpenGL visualization of the Lorenz Attractor. The
lorenz.c  program provides an integrator that may be used to generate a
sequence of points to use in the visualization.

At a minimum, your program should provide a line trace of the sequence of
attractor and allow the trace to be viewed from different positions and allow
one or more of the parameters in the Lorenz equations to be modified
interactively.  (The academic lesson here is what it takes to get a simple
scene rendered and basic user interaction.)

This is your opportunity to experiment and impress your friends with cool
science, so use your imagination and explore both OpenGL and the properties of
the Lorenz Attractor.

What to submit:

1) One ZIP or TAR archive containing all files you are submitting;

2) Source code and Makefile. I'm going to recompile and run this on a
Linux/Ubuntu box so use #ifdef in your code if you use things that are
not portable. (If you don't have access to a Linux box and the GLX code doesn't
work it won't count against you. Note that any changes you made to the gears
program probably will cause problems for me.) ;

3) Provide a README with brief instructions on how to use the program. This
should include instructions on how to change the view, and whatever else the
program does;

4) Optional: If you discovered anything interesting about the Lorenz Attractor
you can attach a brief writeup. If plain text won't do, a PDF file would be
best;

5) Time it took you to complete the assignment.

Before submitting, please consider the following checklist:

1) Make sure your program compiles with no warnings (gcc -Wall is your friend);

2) Make sure that the program behaves correctly when the window is resized;

3) The program should start with something interesting to see - don't make me
work to see something worth while;

4) Make sure the README tells me what buttons to press to make something
happen.

## Homework 3: Scene in 3D
Create an OpenGL program this allows a scene to be viewed in 3D . The program
should allow the scene to be viewed from multiple eye positions directed by
user input.

The scene should consist of several 3D solid objects, and at least two
instances of the same object, but with each instance at a different position,
scale and orientation. The program must create at least one generic object, and
then create each instance by translation, rotation and scaling of the generic
object.

You must generate the objects yourself.  Canned GLU or GLUT objects may not be
used, not may simply load an object generated by Blender or a similar program
from file.  At least one of the objects must be something that is not provided
in the class examples, i.e. not a sphere or a cube.

The program should allow the scene to be viewed from different viewpoints using
the cursor keys or mouse.

What to draw is left to your imagination. You could, for example, create a
scene of a town consisting of a number of houses. The generic instance of house
can be transformed so that each house has a different length, width, height and
color.

What I don NOT want you to draw are pyramids or objects such as tables and
chairs and snowmen created by simply drawing cuboids and spheroids.  None of
these are sufficiently challenging.

The program should instruct OpenGL to remove those parts of the objects that
are obstructed by other objects in the scene.

Think ahead. You may want to build on this program for subsequent assignments.
In particular, be aware that GLUT objects do not support textures, which will
be a problem later on.

What to turn in:
1) Source code including makefile;
2) Readme with instructions;
3) Approximate time it took to complete the assignment.

The purpose of this assignment is to give you some experience with creating
generic 3D objects. You may want to stick to just the orthogonal projection for
this assignment as it is the simplest to use.

## Homework 4: Projections and Navigation
Create an OpenGL program this allows a scene to be viewed in both orthogonal
and perspective projections from multiple eye positions directed by user input.
The program must have three view modes:
1)  Overhead orthogonal;
2)  Overhead perspective;
3)  First person.

You may NOT use the CSCIx229 library for this assignment.

The scene should consist of several 3D solid objects. You may want to simply
expand on Homework 3.  Using GLU and GLUT objects are still prohibited.

The program should allow the scene to be viewed from different viewpoints using
the cursor keys or mouse.  The orthogonal and perspective projections should
allow the entire scene to be viewed from an overhead view.  Although the scene
would look slightly different between the projections, the view should be from
the same vantage point.

The program should allow a third mode which provides for first person
navigation using a perspective projection.  The cursor keys should allow the
user to traverse the scene.

What to turn in:
1) Source code including makefile to build hw4;
2) Readme with instructions;
3) Approximate time it took to complete the assignment.

The purpose of this assignment is to give you some experience with different
projections. While for any project the projection will be dictated by the
specific application, realistic scenes would generally be in perspective,
while orthogonal projections would appear in CAD and similar applications. You
may want to start by getting you scene created in 3D and view it only using
the orthogonal projection, and then add the perspective projection second,and
finally the first person navigation.

WARNING:  Some people really struggle with first person navigation, while
others find it utterly trivial.  Be sure to leave yourself enough time to
figure out which category you fall in.

