## Example1:Solving a differential equation
DSolve[y''[x]-y'[x]-6y[x]==x,y[x],x]

## Example2: Solving a differential equation with a condition
[{y'[x]==y[x],y'[0]==10},y[x],x]

## Example3: assign a variable for a solution of a diff. equ.
diffsol=DSolve[{y'[x]==y[x],y'[0]==10},y[x],x]

## Example4:defining a function for the solution
f[x_]=y[x] /. diffsol

## Example5: Plotting the function
