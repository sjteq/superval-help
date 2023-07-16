# Actives Basis: LateRetirement



## Benefit Accrual after NRA

Check the box if accrual of benefits continues after NRA.

## Salary for Late Retirement

Select from the drop-down list the salary to use for Late Retirement.
The options are:

-   NRA Salary
-   Retirement Salary

If `NRA Salary` is used, specify the increases that should be applied to
salaries after NRA and before actual retirement date in the [Post NRA
Salary Revaluation Rate](actives_basis+lrsalinc.md) on the Salaries
tab.

If `Retirement Salary` is used both the [Salary Increase
Rate](actives_basis+salinc.md) (on the Financial tab) and the
[Promotional Scale Table](actives_basis+sxx.md) (on the Salaries Tab)
will be used to increase the member’s salary up to the member’s actual
retirement.

## Male Retirement Factors  Parameter Set

## Female Retirement Factors  Parameter Set

Retirement Factor Parameter Set is a Scheme Global parameter which
groups the Male or Female Retirement Factor variables. This can be
created by using either the `Create Globals` function or using the
_Add/Edit Retirement Factors_ button. Once created, these parameters
can be edited without going back into the Basis similar to other global
parameter sets.

## Male LRF1 (Revaluation 1 & 3)

## Male LRF1 (Revaluation 2)

## Male LRF2 (Revaluation 1 & 3)

## Male LRF2 (Revaluation 2)

## Female LRF1 (Revaluation 1 & 3)

## Female LRF1 (Revaluation 2)

## Female LRF2 (Revaluation 1 & 3)

## Female LRF2 (Revaluation 2)

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

## LRFs apply to

Select from the drop-down list which benefits the LRF apply to. The
options are:

-   All Pension
-   Pre NRA Accrued Pension

Use `All Pension` if the late retirement factors apply to all the
pension.

Use `Pre NRA Accrued Pension` if the late retirement factors only apply
to the portion accrued up to NRA.

## Apply LRFs to Spouse's

Check this box if you require the spouse’s death after retirement
pension to include the late retirement factors applied to the member’s
pension. Leave the box unchecked if you require the spouse’s death after
retirement pension to be based on member’s pension before the
application of late retirement factors.

## Male COT LRF1 (Revaluation 1 & 3)

## Male COT LRF1 (Revaluation 2)

## Male COT LRF2 (Revaluation 1 & 3)

## Male COT LRF2 (Revaluation 2)

## Female COT LRF1 (Revaluation 1 & 3)

## Female COT LRF1 (Revaluation 2)

## Female COT LRF2 (Revaluation 1 & 3)

## Female COT LRF2 (Revaluation 2)

This field allows the user to specify a set of late retirement
adjustment factors that apply to cash on top options other than `Accrual
&times; Salary for each year`. When using `Accrual × Salary for each year`
SuperVal always assumes the Late Retirement Factors are equal to 1.00.
The user can specify 4 different sets of Late Retirement Factors. These
are:

-   LRF1 for use with Revaluation Rates in deferment 1 and 3
-   LRF1 for use with Revaluation Rate 2
-   LRF2 for use with Revaluation Rates in deferment 1 and 3
-   LRF2 for use with Revaluation Rate 2

Double click to select from a list of available rate tables.

SuperVal assumes exits at NRA and all subsequent ages occur at age exact
(and not half way through the year). Double-click to select from a list
of available rate tables.

Please note that if this field is left blank for cash-on-top benefits
then, for options other than `Accrual × Salary for each year` the LRF
pensions factors will be used. If you do not wish the cash-on-top
benefits to be adjusted, specify a table with all LRFs set to 1.00.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

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