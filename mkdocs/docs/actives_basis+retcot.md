# Actives Basis: RetCOT



## Cash on Top Parameter Set

Cash Parameter Set is a Scheme Global parameter which groups the
Retirement Cash Commutation variables. This can be created by using
either the `Create Globals` function or using the _Add/Edit Retirement
Cash_ button. Once created, these parameters can be edited without going
back into the Basis similar to other global parameter sets.

## Benefit Basis

A lump sum cash benefit can be paid at retirement either through
commutation (ie exchange of pension for cash) or in addition to the
pension benefits. Select from the drop-down list the basis of
calculating any cash benefit provided. The options are:

-   Neutral or Nil
-   25% of Pension
-   IR Maximum
-   2.25 &times; Pension
-   Accrual &times; Salary for each year
-   3 &times; Pension
-   Multiple of Pension
-   % of Pension

When using the `IR Maximum option` the user will need to set up the [IR
Maximum Parameters Rules](actives_basis+irmaxind.md).

When using the `Accrual × Salary for each year`, the user will be
required to enter the salary, service and accrual rate on which this is
based. Note that if using this option, ERF factors will not be applied
to the cash on top lump sum. (If you do want ERFs to be applied to cash
on top, you could use the Multiple of pension option instead.)

When using the `Multiple of Pension`, the Multiple can either be fixed
for all members or be a member specific amount. To use a fixed Multiple,
enter the value. To use a Member Specific Multiple, select from the
drop-down list the data item containing the appropriate data.

When using the `% of Pension`, the Percentage can either be fixed for
all members or be a member specific amount. To use a fixed Percentage,
enter the value. To use a Member Specific Percentage, select from the
drop-down list the data item containing the appropriate data.

When using `25% of Pension` or `% of Pension`, the amount of cash lump
sum will be determined by the Commutation Tables specified.

For all of these options you can select whether to [Ignore GMP in
Split.](actives_basis+cgmp.md) The Commutation will be restricted to
avoid commuting the GMP, however there is no allowance for
post-retirement increases in calculating this restriction. In addition,
you will be required to specify the [Commutation
Priority](bases+cashp.md) and the Commutation Tables to use.

Finally, where benefits for both Cash On Top of pension and Cash
Commutation are specified the Cash Commutation is calculated first. If
the Cash On Top formula relates to the amount of pension this will be
based on the pension prior to commutation.

## Accrual Rate

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Enter the percentage of salary to be
used in the calculation of cash for each year of service i.e. for 3/80ths
use `0.0375`.

When using this option, Early-Retirement Factors will not be applied to
the cash-on-top benefit.

## Salary

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Select from the drop-down list the
salary to be used in the calculation of cash for each year of service.

When using this option, Early-Retirement Factors will not be applied to
the cash-on-top benefit.

## Service

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Select from the drop-down list the
service to be used in the calculation of cash for each year of service.
The options are:

-   Scheme Membership
-   Company Service

Note that total service from either Date Joined Scheme or Date Joined
Company will be used in these calculations.

When using this option, Early-Retirement Factors will not be applied to
the cash-on-top benefit.

## Cash Multiple

This field is only required if the Cash Calculations are based on a
`Multiple of Pension`. The Multiple can either be fixed for all members
or member specific.

To use a fixed multiple, enter the multiple here. (Using a multiple of 3
is the same as selecting `3 &times; pension`.)

To value a member specific multiple, select from the drop-down list the
data item containing the appropriate data.

## Cash Percentage

This field is only required if the Cash Calculations are based on a `%
of Pension`. The Percentage can either be fixed for all members or a
member specific percentage.

To value a fixed percentage for all members, enter the percentage here
ie for 25% enter `0.25`.

To value a member-specific percentage, select from the drop-down list
the data item containing the appropriate data.

## Male Retirement Factors  Parameter Set

## Female Retirement Factors  Parameter Set

Retirement Factor Parameter Set is a Scheme Global parameter which
groups the Male or Female Retirement Factor variables. This can be
created by using either the `Create Globals` function or using the
_Add/Edit Retirement Factors_ button. Once created, these parameters
can be edited without going back into the Basis similar to other global
parameter sets.

## Male COT ERF1 (Revaluation 1 & 3)

## Male COT ERF1 (Revaluation 2)

## Male COT ERF2 (Revaluation 1 & 3)

## Male COT ERF2 (Revaluation 2)

## Female COT ERF1 (Revaluation 1 & 3)

## Female COT ERF1 (Revaluation 2)

## Female COT ERF2 (Revaluation 1 & 3)

## Female COT ERF2 (Revaluation 2)

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

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Decr Help

Rate tables can be selected by any of the following methods:

-   Right-click on the field for a list of appropriate Rate Tables. For
    a field that will accept more than one type of Rate Table (e.g.
    Miscellaneous Tables), the list will be restricted to the current
    Table Type specified in the field – if you wish to see all allowable
    Rate Tables, delete the Table Type from the field before clicking;
    or
-   Double Clicking on the field will produce the Rate Tables form where
    Rate Tables can be viewed (numerically and graphically) and Rate
    Tables can be added or edited. A Rate Table can be selected by
    pressing the Select button or double clicking on the Rate Table
    description in the tree; or
-   the list of allowable Rate Tables can be scrolled through by
    pressing the `<` or `>` keys. The description of the Rate Table to
    the right of the field will change as each new Table is selected.

## Linearly Interpolate Male Retirement Factors for mid-point Exit values

## Linearly Interpolate Female Retirement Factors for mid-point Exit values

When checked, the system will linearly interpolate factors for mid year
exits such as early retirements and deaths. For Normal Retirements, the
system will apply no interpolation. If unchecked, the system will use
the factor specified at the age nearest rounded down for mid year exits
as previous versions have done.

## Add/Edit Retirement Cash

Add or Edit any Retirement Cash parameter sets

## Add/Edit Retirement Factors

Add or Edit any Retirement Factor parameter sets

## SaveAs

Click the _Save As_ button to save with a new file name.

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