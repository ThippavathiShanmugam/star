import turtle as t
t.bgcolor("red")
t.pencolor("black")
t.speed(19)
def shape(angle,side,lim):
    rev_dir=20
    t.forward(side)
    if side % (rev_dir*2)==0:
        angle=angle +2
    t.right(angle)
    side=side+2
    if side <  lim:
        shape(angle,side,lim)
angle=int(input("enter the angle"))
side=int(input("enter the side"))
lim=int(input("enter the lim"))
shape(angle,side,lim)
t.done()

