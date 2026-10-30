# import turtle

screen = turtle.Screen()
screen.bgcolor('grey')
pen = turtle.Turtle()

pen.speed(0)
pen.hideturtle()

def draw_rectangle(colour, x, y, width, height):
  pen.penup()
  pen.goto(x,y)
  pen.pendown()
  pen.color(colour)
  pen.begin_fill()
  
  for i in range(2):
    pen.forward(width)
    pen.right(90)
    pen.forward(height)
    pen.right(90)
  

  pen.end_fill()  
def draw_circle(colour, x, y):
  pen.penup()
  pen.goto(x,y)
  pen.pendown()
  pen.color(colour)
  pen.begin_fill()
  pen.circle(30)
  pen.end_fill()
  
draw_rectangle('black', -50, 150, 100, 300)
draw_circle('red', -30, 85)
draw_circle('yellow', -30, -15)
draw_circle('green', -30, -115)
draw_rectangle('grey', -10, -150, 20, 100)

turtle.done()
