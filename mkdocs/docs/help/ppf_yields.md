# PPF Yields



## Applicable Date

Enter the date at which the PPF Yields are applicable. The format must
be DD/MM/YYYY.

## Secondary Key (Optional)

The Secondary Key can be used to distinguish between different yields
that apply at the same valuation date i.e. where yields are dependent on
the date the PPF S179 (Levy) Valuation will be signed.

The user can use the Secondary Key to enter a description of the
appropriate yields i.e. `GNV2 (Pre 1 Nov 06)`. This can be either a
numeric value or a description and up to 20 characters in length.

When selecting the yields in the Scheme PPF tab, both the yield date and
the Secondary Field narrative are visible.

## Index- Linked 5yrs 5%

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

## Index- Linked 5yrs 0%

## Index Linked over 5 years 0% Inflation

Enter the FTSE Index Linked over 5 years 0% inflation Gilt Yield as at
the Applicable Date. (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield C (pre 31 March 2008
valuations) and Yield D (post 30 March 2008 valuations).  The Yields are
calculated as follows:

$$\frac{\left[ \left( 1 + \frac{I - L_{5yrs 5\%}}{2} \right)^2 -1 \right] + \left[ \left( 1 + \frac{I - L_{5yrs 0\%}}{2} \right)^2 -1 \right]}{2}$$


<!-- 0.5 x { \[(1 + 0.5 x I-L 5yrs 5%)^2 - 1\] + \[(1 + 0.5 x I-L 5yrs 0%)^2 - 1\] } -->

The adjustment required to both Yield C (pre 31 March 2008 valuations)
and Yield D (post 30 March 2008 valuations) is documented in the
Guidance from the PPF and is determined by the date of valuation. 
SuperVal automatically allows for the adjustments documented in Guidance
Note A3, A4, A5, A6, A7, A8 and A9.  

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.

## Index- Linked 5-15yrs 5%

Enter the FTSE Index Linked for 5 - 15 years 5% inflation Gilt Yield as
at the Applicable Date. (SuperVal will calculate the annualised yield.)

## Index- Linked 5-15yrs 0%

Enter the FTSE Index Linked for 5 - 15 years 0% inflation Gilt Yield as
at the Applicable Date. (SuperVal will calculate the annualised yield.)

## Index- Linked 15yrs 5%

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

## Index- Linked 15yrs 0%

## Index Linked over 15 years 0% Inflation

Enter the FTSE Index Linked over 15 years 0% inflation Gilt Yield as at
the Applicable Date.  (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield A.  Yield A is
calculated as follows:

$$\frac{\left[ \left( 1 + \frac{I - L_{15yrs 5\%}}{2} \right)^2 -1 \right] + \left[ \left( 1 + \frac{I - L_{15yrs 0\%}}{2} \right)^2 -1 \right]}{2}$$

The adjustment required to Yield A is documented in the Guidance from
the PPF and is determined by the date of valuation.  SuperVal
automatically allows for the adjustments documented in Guidance Notes
A3, A4, A5, A6, A7, A8 and A9.  

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.

## Fixed 10yrs

## Fixed Interest 10 years Gilt Yield

Enter the FTSE Fixed Interest 10 year Gilt Yield as at the Applicable
Date. (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield B (pre 31 March 2008
valuations) and Yield C (valuations between 31 March 2008 and 30 October
2009).  The annualised yield will be calculated as follows:

$$\left( 1 + \frac{Fixed Interest_{10yr Yield}}{2} \right)^{2} - 1$$

The adjustment required to Yield B (pre 31 March 2008 valuations) and
Yield C (valuations between 31 March 2008 and 30 October 2009) is
documented in the Guidance from the PPF and is determined by the date of
valuation.  SuperVal automatically allows for the adjustments documented
in Guidance Note A3, A4, A5, A6, A7, A8 and A9.     

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.

## Fixed 15yrs

## Fixed Interest 15 years Gilt Yield

Enter the FTSE Fixed Interest 15 year Gilt Yield as at the Applicable
Date. (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield C (post 30 October
2009 valuations).  The annualised yield will be calculated as follows:

$$\left( 1 + \frac{Fixed Interest_{15yr Yield}}{2} \right)^{2} - 1$$

The adjustment required to Yield C (post 30 October 2009 valuations) is
documented in the Guidance from the PPF and is determined by the date of
valuation.  SuperVal automatically allows for the adjustments documented
in Guidance Note A3, A4, A5, A6, A7, A8 and A9.     

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.

## Fixed 20yrs

## Fixed Interest 20 years Gilt Yield

Enter the FTSE Fixed Interest 20 year Gilt Yield as at the Applicable
Date. (SuperVal will calculate the annualised yield.)

This yield will be used in the calculation of Yield B (post 30 March
2008 valuations).  Yield B (post 30 March 2008 valuations) is calculated
as follows:

$$\left( 1 + \frac{Fixed Interest_{20yr Yield}}{2} \right)^2 -1 $$
<!-- 
(1 + 0.5 x Fixed Interest 20yr Yield) ^ 2 - 1
 -->

The adjustment required to Yield B (post 30 March 2008) is documented in
the Guidance from the PPF and is determined by the date of valuation. 
SuperVal automatically allows for the adjustments documented in Guidance
Note A3, A4, A5, A6, A7, A8 and A9.     

The yield is entered as a percentage, i.e. for 3% enter `3` and not `0.03`.

## Pre Retirement Adjustment

## PPF Yields – Pre 2009 Pre Retirement Adjustment

SuperVal calculates the PPF yields in accordance with the Guidance
issued from the PPF and documented in Guidance Notes A3, A4, A5, A6, A7,
A8 and A9.  

This field can be used to make adjustment to this calculation i.e. to
reflect Guidance prior to A3 or when new Guidance is issued.  

Enter the adjustment that applies to the yield used for compensation
increasing in deferment and accrued before 6 April 2009. The adjustment
is additive, i.e. if the calculated yield is 3.25% and `0.25` is entered, the
revised yield will be 3.50%.

## Post 2009 Pre Retirement Adjustment

SuperVal calculates the PPF yields in accordance with the Guidance
issued from the PPF and documented in Guidance Notes A3, A4, A5, A6 and
A7.

This field can be used to make adjustment to this calculation i.e. to
reflect Guidance prior to A3 or when new Guidance is issued.

Enter the adjustment that applies to the yield used for compensation
increasing in deferment and accrued after 5 April 2009. The adjustment
is additive i.e. if the calculated yield is 3.25% and `0.25` is entered, the
revised yield will be 3.50%.

## Pensioner Post Retirement (With Increases) Adjustment

SuperVal calculates the PPF yields in accordance with the Guidance
issued from the PPF and documented in Guidance Notes A3, A4, A5, A6, A7,
A8 and A9.

This field can be used to make adjustment to this calculation, i.e. to
reflect Guidance prior to A3 or when new Guidance is issued.

Enter the adjustment that applies to the yield used for compensation
with increases in payment. The adjustment is additive, i.e. if the
calculated yield is 3.25% and `0.25` is entered; the revised yield will be
3.50%.

## Pensioner Post Retirement (No Increases) Adjustment

SuperVal calculates the PPF yields in accordance with the Guidance issued from the PPF and documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9.

This field can be used to make adjustment to this calculation, i.e. to reflect Guidance prior to A3 or when new Guidance is issued.

Enter the adjustment that applies to the yield used for compensation with no
increases in payment. The adjustment is additive, i.e. if the calculated
yield is 3.25% and `0.25` is entered; the revised yield will be
3.50%.

## Non-Pensioner Post Retirement (With Increases) Adjustment

## PPF Yields - Post Retirement (with increases) Adjustment

SuperVal calculates the PPF yields in accordance with the Guidance issued from the PPF and documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9.

This field can be used to make adjustment to this calculation, i.e. to reflect Guidance prior to A3 or when new Guidance is issued. 

Enter the adjustment that applies to the yield used for compensation
with increases in payment.  The adjustment is additive, i.e. if the calculated yield is 3.25% and `0.25` is entered, the revised yield will be 3.50%.

## Non-Pensioner Post Retirement (No Increases) Adjustment

## PPF Yields - Post Retirement (no increases) Adjustment

SuperVal calculates the PPF yields in accordance with the Guidance issued from the PPF  and documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9. 

This field can be used to make adjustment to this calculation, i.e. to reflect Guidance prior to A3 or when new Guidance is issued.

Enter the adjustment that applies to the yield used for compensation
with no increases in payment. The adjustment is additive, i.e. if the
calculated yield is 3.25% and `0.25` is entered, the revised yield will be
3.50%.

## Pre Retirement

## PPF Yields - Pre Retirement

SuperVal shows you the net yield that will be used to value compensation
increasing in deferment and accrued prior to 6 April 2009.  

The yield will be calculated in accordance with the Guidance issued from
the PPF documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9 and
then adjusted by any entry in the Pre Retirement Adjustment field.

## Post 2009 Pre Retirement

## PPF Yields - Post 2009 Pre-Retirement

SuperVal shows you the net yield that will be used to value compensation
increasing in deferment and accrued post 6 April 2009.  

The yield will be calculated in accordance with the Guidance issued from
the PPF documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9 and
then adjusted by any entry in the Post 2009 Pre Retirement Adjustment
field.

## Pensioner Post Retirement (With Increases)

SuperVal shows you the net yield that will be used to value pensions
with increases in payment.

The yield will be calculated in accordance with the Guidance issued from
the PPF documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9 and
then adjusted by any entry in the Post Retirement (with increases)
Adjustment field.

## Pensioner Post Retirement (No Increases)

SuperVal shows you the net yield that will be used to value pensions
with no increases in payment.

The yield will be calculated in accordance with the Guidance issued from
the PPF documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9 and
then adjusted by any entry in the Post Retirement (No Increases)
Adjustment field.

## Non-Pensioner Post Retirement (With Increases)

## PPF Yields - Post Retirement (with increases)  

SuperVal shows you the net yield that will be used to value pensions
with increases in payment.   

The yield will be calculated in accordance with the Guidance issued from
the PPF documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9 and
then adjusted by any entry in the Post Retirement (with increases)
Adjustment field.

## Non-Pensioner Post Retirement (No Increases)

## PPF Yields - Post Retirement (No Increases)  

SuperVal shows you the net yield that will be used to value pensions
with no increases in payment.   
  
The yield will be calculated in accordance with the Guidance issued from
the PPF documented in Guidance Notes A3, A4, A5, A6, A7, A8 and A9 and
then adjusted by any entry in the Post Retirement (No Increases)
Adjustment field.

## Grid Help

Right-clicking on a column heading presents a menu with the following
options which allow you to expand or reduce the number of columns of
data to be entered:

-   Add a new column to the right of the grid;
-   Insert a new column at the position of the cursor; and
-   Delete the current column at the position of the cursor.

## Grid Help

Right-clicking on the Top Left Corner of the grid displays a menu which
allows you to set the following Grid Editing Options:

-   Editing of a cell can be invoked by either clicking on the cell or
    by pressing F2 when the cell is active (Clicking will only change
    the current active cell); and
-   determine the cursor movement once editing is complete to be either
    to the next cell down, the next cell to the right or to stay in the
    current cell.

## Delete Row

Click here to delete an existing row of PPF yields or PPF Caps.

## Edit Row

Click here to edit an existing row of PPF Yields or PPF Caps.

## Add Row(s)

Click here to add an additional row of PPF Yields or PPF Caps.

## Save

Clicking on the _Save_ button allows you to save the entries.

## Quit

Clicking on the _Quit_ button allows you to exit without saving any of
your changes.

In some of the screens you will be asked to confirm if you want to exit
_Ignoring all changes_. If you click _Yes_, the file will be closed
without saving any changes. If you click _No_ you will be returned to your
original screen.

From the Browser, the _Quit_ button will take you to a graphical display
of the results.