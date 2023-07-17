# Early-Retirement Factors: Cash on Top

This field allows the user to specify a set of early retirement
reduction factors that apply to cash-on-top benefits options other than
`Accrual × Salary for each year`. When using `Accrual × Salary for each
year` SuperVal always assumes the Early-Retirement Factors are equal to
1.00. The user can specify 4 different sets of Early-Retirement Factors.
These are:

-   ERF1 for use with Revaluation Rates in deferments 1 and 3
-   ERF1 for use with Revaluation Rate 2
-   ERF2 for use with Revaluation Rates in deferment 1 and 3
-   ERF2 for use with Revaluation Rate 2


## Users without access to Late Retirement Code

The rate table is typically an `FX` table and should contain non-zero
entries for ages at which members are assumed to retire. Please note
that SuperVal assumes exits prior to NRA occur half-way through the year
ie 0.5 years, 1.5 years etc after the valuation date. Exits at NRA occur
at the beginning of the year. This should be reflected in the
early-retirement reduction factor tables used. Therefore, if the
reduction is 4% simple per annum, and the NRA is 65, the table should be
defined as follows:

Age  | Rate
-----|-----
65   | 1.00
64   | 0.98
63   | 0.94
62   | 0.90
Etc. |

Benefits of member’s above NRA can be adjusted to reflect late payment
by adding a factor in ages above NRA i.e. 1.04 at age 66 for a 4%
increase. Please note members above NRA will be assumed to retire at the
valuation date.

Where this has been left blank, SuperVal will use the Pension
Early-Retirement Factors specified. (To value an unreduced cash payment
enter a table with 1.00 at each age.)

Double-click to select from a list of available rate tables.


## Users with access to Late Retirement Code

The rate table is typically an `FX` table and should contain non-zero
entries for ages at which members are assumed to retire. If a LRA is
specified, SuperVal will only use the table specified here prior to NRA.

Please note that SuperVal assumes exits prior to NRA occur half-way
through the year i.e. 0.5 years, 1.5 years etc after the valuation date.
Exits at NRA occur at the beginning of the year. This should be
reflected in the early-retirement reduction factor tables used.
Therefore, if the reduction is 4% simple per annum, and the NRA is 65,
the table should be defined as follows:

Age  | Rate
-----|-----
65   | 1.00
64   | 0.98
63   | 0.94
62   | 0.90
Etc. | 

Where a Late Retirement Age has not been specified, members above NRA
will be assumed to retire immediately using the ERF specified here. If
this has been left blank, SuperVal will use the Pensions ERF specified.
(To value an unreduced cash payment enter a table with 1.00 at each
age.)

Where a Late Retirement Age has been specified, members above NRA will
be assumed to retire in accordance with the ER/LR decrement specified on
the Demographic Tab. Please note all retirements after NRA occur at the
beginning of the year. Their benefits above NRA will be adjusted using
the Cash on Top Late Retirement Factors specified on the Late Retirement
Tab. Where this field has been left blank, SuperVal will use the Pension
Early/Late Retirement Factors specified. (To value an unreduced cash
payment enter a table with 1.00 at each age.)

Double-click to select from a list of available rate tables.
