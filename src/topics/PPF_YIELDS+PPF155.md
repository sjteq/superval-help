# PPF_Yields+PPF155



## Index Linked over 15 years 5% Inflation

Enter the FTSE Index Linked over 15 years 5% inflation Gilt Yield as at
the Applicable Date.  (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield A.  Yield A is
calculated as follows:

$$\frac{\left[ \left( 1 + \frac{I - L_{15yrs 5\%}}{2} \right)^2 -1 \right] + \left[ \left( 1 + \frac{I - L_{15yrs 0\%}}{2} \right)^2 -1 \right]}{2}$$

<!-- 
0.5 x { [(1 + 0.5 x I-L 15yrs 5%)^2 - 1] + [(1 + 0.5 x I-L 15yrs 0%)^2 - 1] }

```q
(%2)sum(-1)xexp[;2]1+0.5*I-L[15;5 0]
```
 -->
The adjustment required to Yield A is documented in the Guidance from
the PPF and is determined by the date of valuation.  SuperVal
automatically allows for the adjustments documented in Guidance Notes
A3, A4, A5, A6, A7, A8 and A9.  

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.  

