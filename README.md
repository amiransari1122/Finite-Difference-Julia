# Finite-Difference-Julia
This is a finite differences implementation  in Julia Language.

This function can take a Tabular Function like (X,Y) and interpolate some points like  xn that are in bounds of X, 
you can try either forward ( if your points are near to X(1) ) and backward( if your points are near to X(end) );

X,Y are points of a Table Function to Interpolation,
xn are new points that must be in X's range and
"kind" parameter specifies type of finite difference.[ forward / backward ]

I divided the algorithm to two parts and took "t" and "d" matrices that "t" is Bionomial Coefficients and "d" is Differences Matrix .
Last of algorithm ,by multipling t * f( and b for backwarding),xn values are calculated.

f is first row of d for forward moving and b is last row of it.
