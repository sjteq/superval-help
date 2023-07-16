# Interpolate_Rates+nra

Use this functionality to create Exact-Age rates $y$ from mid-Year rates
$x$.

Exact-Age rates are calculated as follows:

$$y(NRA) = x(NRA)$$

$$y(NRA-1) = 2x(NRA) - y(NRA)$$

$$y(NRA-2) = 2x(NRA-1) - y(NRA-1)$$

...

