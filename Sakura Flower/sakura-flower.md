## Source code for sakura flower mandala art
```python
from turtle import *
bgcolor('black')
pencolor('white')
fillcolor('#dce3f1')
speed(0)
def flower():
    pensize(3)
    pencolor('#d8697b')
    for i in range(10):
        rad=90
        for i in range(10):
            circle(rad)
            rad-=4
        right(36)  
def pentago():
    pencolor('#ed8945')
    pensize(2)
    fillcolor('#f0bbb8')
    begin_fill()
    for i in range(6):
        for i in range(5):
            right(75)
            forward(200)
        right(45)
    end_fill()
def star():
    pencolor('white')
    fillcolor('#ed8945')
    begin_fill()
    for i in range(9):
        fd(80)
        left(160)
    end_fill()
    
penup()
goto(-10,-320)
pd()
begin_fill()
circle(radius=290)
end_fill()
penup()
goto(0,0)
pd()
pentago()
penup()
goto(-5,-40)
pd()
flower()
penup()
goto(0,-80)
pd()
pencolor('#ed8945')
fillcolor('#dce3f1')
begin_fill()
circle(radius=46)
end_fill()
penup()
goto(-40,-40)
pd()
pensize(0)
star()
hideturtle()

done()

