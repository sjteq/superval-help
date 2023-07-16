# Late Retirement Factors: Benefits

This field allows the user to specify a set of late retirement
adjustment factors that apply to benefits. The user can specify 4
different sets of Late Retirement Factors. These are:

-   LRF1 for use with Revaluation Rates in deferment 1 and 3
-   LRF1 for use with Revaluation Rate 2
-   LRF2 for use with Revaluation Rates in deferment 1 and 3
-   LRF2 for use with Revaluation Rate 2

There should be non-zero entries for all ages at which members are
assumed to retire.

SuperVal assumes exits at NRA and all subsequent ages occur at age exact
(and not half way through the year). Double-click to select from a list
of available rate tables.

Benefits of members above LRA can be adjusted to reflect late payment by
adding a factor in ages above LRA. Please note members above LRA will be
assumed to retire at the valuation date.

If this field is left bank, and a Late Retirement decrement is used,
then SuperVal will assume a LRF equal to 1.

Please note that if the separate Late Retirement Factors for cash-on-top
benefits are left blank then, for options other than `Accrual × Salary
for each year` then the factor specifed here for pensions will be used.
