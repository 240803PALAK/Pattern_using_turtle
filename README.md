# Pattern_using_turtle
using turtle library forming the patterns.


    import turtle
    tk=turtle.Turtle()
    # Square
    tk.color("blue","#3C9118")
    
    tk.begin_fill()
    tk.forward(100)
    tk.left(90)
    tk.forward(100)
    tk.left(90)
    tk.forward(100)
    tk.left(90)
    tk.forward(100)
    
    tk.penup()
    tk.forward(100)
    tk.pendown()
    
    tk.forward(100)
    tk.left(90)
    tk.forward(100)
    tk.left(90)
    tk.forward(100)
    tk.left(90)
    tk.forward(100)
    tk.left(90)
    tk.end_fill()
    
    turtle.done()
    
    
    
    
    import turtle
    tk=turtle.Turtle()
    
    tk.color("red")
    tk.speed(10)
    for i in range(100):
        tk.forward(300)
        tk.left(170)
    turtle.done()
    
    
    
    
    import turtle
    import math
    tk=turtle.Turtle()
    tk.color("red","yellow")
    tk.speed(10)
    
    for i in range(1000):
        tk.forward(math.sqrt(i))
        tk.left(i%180)
    turtle.done()
    
    
    
    
    import turtle
    import math
    tk=turtle.Turtle()
    tk.color("cyan","yellow")
    tk.speed(10)
    
    for i in range(1000):
        tk.forward(math.sqrt(i/10)*25)
        tk.left(20)
    turtle.done()
    
    
    
    
    import turtle
    tk=turtle.Turtle()
    tk.getscreen().bgcolor("#3C9118")
    tk.color("red","yellow")
    tk.penup()
    tk.goto((-200,100))
    tk.pendown()
    tk.speed(10)
    def start(size):
        if size<=10:
            return
        else:
            tk.begin_fill()
            for i in range(5):
                tk.forward(size)
                start(size/3)
                tk.left(216)
            tk.end_fill()
    start(360)
    turtle.done()
