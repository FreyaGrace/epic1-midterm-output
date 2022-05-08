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
  
          
           
rays()

turtle.done()
