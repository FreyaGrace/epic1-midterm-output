# Source Code for the Sun mandala art design

```python
import turtle
turtle.bgcolor('black')
turtle.speed(0)
turtle.pensize()

def rays():
    colors = ('#da9100','#ffdf00')

    for i in range (200):
        turtle.forward(i*4)
        turtle.right(91)
        turtle.color(colors[i%2])
    
        for x in range(3):
          turtle.forward(x*4)
          turtle.right(91)

          for a in range(2):
               turtle.forward(a*4)
               turtle.right(91)
  
def flower_of_life():
  turtle.pensize(3)
  turtle.pencolor('#840602')
  for x in range(6):

    turtle.circle(100)

    turtle.left(60)

rays()
turtle.pu()
turtle.goto(0,0)
turtle.pd()
flower_of_life()

turtle.pu()
turtle.pensize(4)
turtle.pencolor('#e6ac03')
turtle.goto(30,100)
turtle.pd()
turtle.circle(100)
turtle.pu()
turtle.goto(70,190)
turtle.pd()
turtle.circle(210)
turtle.pu()
turtle.goto(75,210)
turtle.pd()
turtle.circle(230)
turtle.hideturtle()
turtle.done()
