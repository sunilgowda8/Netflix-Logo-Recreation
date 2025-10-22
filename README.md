# Draw Netflix Logo

In this tutorial, we will be learning how to draw Netflix logo using Python Turtle. We’ll divide the process into 3 parts, and explain each one of them.

## Import the module and initialize it

```
import turtle
from time import sleep

# Part 1 : Initialize the module
t = turtle.Turtle()
t.speed(4)
turtle.bgcolor("white")
t.color("white")
turtle.title('Netflix Logo')
```

What we are doing here is basically importing the ‘turtle’ module, initializing it using ‘turtle.Turtle()’, then setting our configuration, like the drawing speed, the main window background color, the trace color of the turtle, and the title of the drawing window.

## Draw the logo black background

As we all know, the Netflix logo has a black square background rounded on the borders. So let’s draw it.

```
# Part 2 : Drawing the black background
t.up()
t.goto(-80,50)
t.down()
t.fillcolor("black")
t.begin_fill()

t.forward(200)
t.setheading(270)
s = 360
for i in range(9):
    s = s - 10
    t.setheading(s)
    t.forward(10)
    
t.forward(180)
s = 270
for i in range(9):
    s = s - 10
    t.setheading(s)
    t.forward(10)

t.forward(200)
s = 180
for i in range(9):
    s = s - 10
    t.setheading(s)
    t.forward(10)

t.forward(180)
s = 90
for i in range(9):
    s = s - 10
    t.setheading(s)
    t.forward(10)
t.forward(30)    
t.end_fill()
```

What we are doing here is drawing the black background square by tracing 4 lines, and at the same time making rounded borders using a loop on each corner.

## Complete the logo

We’re almost done! Drawing the letter N that stands for Netflix is the only thing left. This is the most important part of our article to Draw Netflix logo.

```
# Part 3 : Drawing the N shape
t.up()
t.color("black")
t.setheading(270)
t.forward(240)
t.setheading(0)
t.down()
t.color("red")
t.fillcolor("#E50914")
t.begin_fill()
t.forward(30)
t.setheading(90)
t.forward(180)
t.setheading(180)
t.forward(30)
t.setheading(270)
t.forward(180)
t.end_fill()
t.setheading(0)
t.up()
t.forward(75)
t.down()
t.color("red")
t.fillcolor("#E50914")
t.begin_fill()
t.forward(30)
t.setheading(90)
t.forward(180)
t.setheading(180)
t.forward(30)
t.setheading(270)
t.forward(180)
t.end_fill()
t.color("red")
t.fillcolor("red")
t.begin_fill()
t.setheading(113)
t.forward(195)
t.setheading(0)
t.forward(31)
t.setheading(293)
t.forward(196)
t.end_fill()
t.hideturtle()
sleep(10)
```

First, we changed the turtle trace color from white (in part 1) to black so we don’t leave white traces on the black background. Then, we placed the turtle in the position where we should start drawing the shape and changed the trace color to red. Finally, we drew 3 rectangles: 2 that are parallel to each other and the third one connected them.
#Python #Programming #TurtleGraphics #Netflix #LogoDesign #Coding #CreativeCoding #SoftwareDevelopment #PythonProjects #TechPortfolio

