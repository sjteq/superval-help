# Deferreds Basis: RetCOT



## Cash Parameter Set

Cash Parameter Set is a Scheme Global parameter which groups the
Retirement Cash Commutation variables. This can be created by using
either the `Create Globals` function or using the _Add/Edit Retirement
Cash_ button. Once created, these parameters can be edited without going
back into the Basis similar to other global parameter sets.

## Benefit Basis

Benefit Basis can be Neutral/Nil, Multiple of Pension or Percentage of
Pension.

## Cash Data Field

## Cash Multiple

## Cash Percentage

The cash on top can be calculated either as a Multiple, a Percentage of
the PUP or a Member Specific Amount of Cash.

If an entry is made in the Multiple field, the cash on top cash will be
calculated as:

Multiple &times; PUP revalued to retirement &times; Early Retirement Reduction
Factor (if applicable).

The Multiple can either be a fixed Multiple for all members or a Member
Specific Multiple. To use a fixed Multiple enter the value i.e. for 4
times the PUP enter `4`. To use a Member Specific Multiple, select from
the drop-down list the data item containing the appropriate value. To
value commutation of 4 times the PUP ensure the data item contains the
value 4.

To value a Percentage, ensure the entry in the Multiple field is blank.
The cash on top will be calculated as:

Percentage &times; PUP revalued to retirement &times; Commutation Factor &times; Early
Retirement Reduction Factor (if applicable).

The Percentage can either be a fixed Percentage for all members or a
Member Specific Percentage. To use a fixed Percentage enter the value ie
for 25% enter `25`. To use a Member Specific Percentage, select from the
drop-down list the data item containing the appropriate value. To value
commutation of 25% of the PUP ensure the data item contains the value
25.

To value a Cash Data Item for cash on top, ensure the entry for both the
Multiple and the Percentage fields are blank. Select from the drop-down
list the data item containing the amount of Cash on Top payable for each
member. The lump sum will be revalued in line with the assumption for
[Excess Revaluations](deferreds_basis+revn.md) specified on the
Financial Tab between date of valuation and retirement. For retirements
prior to NRA the benefit will be reduced in line with
[ERFs](#deferreds_basis+ertabc) specified for Cash on Top.

## Male Retirement Factors  Parameter Set

## Female Retirement Factors  Parameter Set

Retirement Factor Parameter Set is a Scheme Global parameter which
groups the Male or Female Retirement Factor variables. This can be
created by using either the `Create Globals` function or using the
_Add/Edit Retirement Factors_ button. Once created, these parameters
can be edited without going back into the Basis similar to other global
parameter sets.

## Male ERF1

## Male ERF2

## Female ERF1

## Female ERF2

## Actives

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
entries for ages at which members are assumed to retire. SuperVal will
only use the table specified here prior to NRA.

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
will be assumed to retire immediately with an ERF of 1 applied to their
benefit.

Where a Late Retirement Age has been specified, members above NRA will
be assumed to retire in accordance with the ER/LR decrement specified on
the Demographic Tab. Please note all retirements after NRA occur at the
beginning of the year. Their benefits above NRA will be adjusted using
the Late Retirement Factors specified on the Late Retirement Tab.

Where this has been left blank, SuperVal will use the Pension
Early-Retirement Factors specified. (To value an unreduced cash payment
enter a table with 1.00 at each age.)

Double-click to select from a list of available rate tables.
**Deferreds**

This field allows the user to specify a set of early retirement
reduction factors that apply to cash-on-top benefits options. The user
can specify 2 different sets of Early-Retirement Factors. These are:

-   ERF1
-   ERF2

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

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

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