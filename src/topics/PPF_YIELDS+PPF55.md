# PPF_Yields+PPF55


## Index Linked over 5 years 5% Inflation

Enter the FTSE Index Linked over 5 years 5% inflation Gilt Yield as at
the Applicable Date. (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield C (pre 31 March 2008
valuations) and Yield D (post 30 March 2008 valuations).  The annualised
yields are calculated as follows:

$$\frac{\left[ \left( 1 + \frac{I - L_{5yrs 5\%}}{2} \right)^2 -1 \right] + \left[ \left( 1 + \frac{I - L_{5yrs 0\%}}{2} \right)^2 -1 \right]}{2}$$

<!-- 
0.5 x { \[(1 + 0.5 x I-L 5yrs 5%)^2 - 1\] + \[(1 + 0.5 x I-L 5yrs 0%)^2 - 1\] }
 -->

The adjustment required to both Yield C (pre 31 March 2008 valuations)
and Yield D (post 30 March 2008 valuations) is documented in the
Guidance from the PPF and is determined by the date of valuation. 
SuperVal automatically allows for the adjustments documented in Guidance
Note A3, A4, A5, A6, A7, A8 and A9.     

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.
