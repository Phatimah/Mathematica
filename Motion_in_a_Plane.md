In this case, the position of the object at time t has both a horizontal component, x(t), and a vertical component, y(t), given by the following:
x(t) = x0 + v0 cos( ) t
y(t) = -1/2 g t2 + v0 sin( ) t + y0.


### Example1
Suppose that a rock is thrown upward at 40 feet/sec at an angle of 30°= /6radians, with respect to the horizontal, and from a height of 20feet.
a) Use Mathematica to plot the position of the rock through space.
b) 

Solution:
https://www.wolframcloud.com/obj/0bf156cb-b1f3-4b42-9310-d0b5a7054a13



### Example2
For the path of the rock from the previous example, approximate the time that the rock reaches its maximum height and the time that the rock reaches the ground by plotting a graph of the position of the rock at time t = 0.0 sec, 0.1 sec, 0.2 sec, 0.3 sec, ..., on the interval [0, 2].

Solution:
https://www.wolframcloud.com/obj/2b3bbd7c-15cd-4073-bdae-f369117affd2

### Example3
Suppose that a rock is thrown upward at 40 feet/sec at an angle of , with respect to the horizontal, and from a height of 20 feet. Let us see how changing the value of the angle,     , affects the path of the rock.

Solution:
In[5]:= x[t_,theta_]=40*Cos[theta]*t;
y[t_,theta_]=-16*t^2+40*Sin[theta]*t+20;
In[6]:= Manipulate[ParametricPlot[{x[t,θ],y[t,θ]},{t,0,3}, PlotRange->{{0,80},{0,60}},PlotLabel-deg],{θ,0,Pi/2,Pi/36}]
