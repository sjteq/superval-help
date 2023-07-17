# Actives Basis: RetPension



## Male Spouse's Reversion

## Female Spouse's Reversion

The field determines the proportion of pension paid to a spouse in the
event of the member’s death in retirement ( i.e. normal, early or ill
health retirement). This can either be a fixed percentage for all
members or a member specific percentage.

To value a fixed percentage for all members enter the figure here. For
50% enter `50`.

To value a member specific percentage, select from the drop-down list
the data item containing the member specific spouse’s proportion. The
data item should be in the form of a percentage so for 50% enter `50`.

Users will have the option to override this value on the Slices or PUPs
Tab for a particular benefit.

## Apply Early Retirement Factor to Spouse's Pension

Check this box if the spouse’s death after retirement pension should be
reduced to reflect the early retirement reduction factor applied to the
member’s pension. Leave the box unchecked if the spouse’s death after
retirement pension is based on member’s pension prior to application of
any early retirement reduction factors.

## Spouse's Pension based on Pre Commutation Pension

Check this box if the spouse’s death after retirement pension is based
on the member’s pre-commutation pension. Leave the box unchecked if the
spouse’s death after retirement pension is based on member’s
post-commutation pension.

## Male Retirement Factors  Parameter Set

## Female Retirement Factors  Parameter Set

Retirement Factor Parameter Set is a Scheme Global parameter which
groups the Male or Female Retirement Factor variables. This can be
created by using either the `Create Globals` function or using the
_Add/Edit Retirement Factors_ button. Once created, these parameters
can be edited without going back into the Basis similar to other global
parameter sets.

## Male ERF1 (Revaluation 1 & 3)

## Male ERF1 (Revaluation 2)

## Male ERF2 (Revaluation 1 & 3)

## Male ERF2 (Revaluation 2)

## Female ERF1 (Revaluation 1 & 3)

## Female ERF1 (Revaluation 2)

## Female ERF2 (Revaluation 1 & 3)

## Female ERF2 (Revaluation 2)

This field allows the user to specify a set of early retirement
reduction factors that apply to pension benefits. The user can specify 4
different sets of Early-Retirement Factors (actives) and 2 different
sets of Early-Retirement Factors (deferreds). For actives these are:

-   ERF1 for use with Revaluation Rates in deferments 1 and 3
-   ERF1 for use with Revaluation Rate 2
-   ERF2 for use with Revaluation Rates in deferment 1 and 3
-   ERF2 for use with Revaluation Rate 2

For deferreds these are

-   ERF1
-   ERF2

## Users without Late Retirement Tab

The rate table is typically an `FX` table and should contain non-zero
entries for ages at which members are assumed to retire. Please note
that SuperVal assumes exits prior to NRA occur half-way through the year
ie 0.5 years, 1.5 years etc after the valuation date. Exits at NRA occur
at the beginning of the year. This should be reflected in the early
retirement reduction factor tables used. Therefore, if the reduction is
4% simple per annum, and the NRA is 65, the table should be defined as
follows:

Age  | Rate
-----|-----
65   | 1.00
64   | 0.98
63   | 0.94
62   | 0.90
Etc. | 

Benefits of members above NRA can be adjusted to reflect late payment by
adding a factor in ages above NRA i.e. 1.04 at age 66 for a 4% increase.
Please note members above NRA will be assumed to retire at the valuation
date.

Where this has been left blank, SuperVal will assume an Early-Retirement
Factor of 1.

Double-click to select from a list of available rate tables.


## Users with Late Retirement Tab

The rate table is typically an `FX` table and should contain non-zero
entries for ages at which members are assumed to retire. Please note
that SuperVal assumes exits prior to NRA occur half-way through the year
ie 0.5 years, 1.5 years etc after the valuation date. Exits at NRA occur
at the beginning of the year. This should be reflected in the early
retirement reduction factor tables used. Therefore, if the reduction is
4% simple per annum, and the NRA is 65, the table should be defined as
follows:

Age  | Rate
-----|-----
65   | 1.00
64   | 0.98
63   | 0.94
62   | 0.90
Etc. | 

If a Late Retirement Age is specified SuperVal will only use the table
specified here up to NRA. Members above NRA will be assumed to retire in
accordance with the ER/LR decrement specified on the Demographic Tab.
Please note all retirements after NRA occur at the beginning of the
year. Their benefits above NRA will be adjusted using the [Late
Retirement Factors](actives_basis+lrtab.md) specified on the Late
Retirement Tab. Where this has been left blank, SuperVal will assume an
Late Retirement Factor of 1.

Where a Late Retirement Age has not been specified, members above NRA
will be assumed to retire immediately using the ERFs specified here.
Where this has been left blank, SuperVal will assume an Early-Retirement
Factor of 1.

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

## Delayed Increases in Payment

Check this box to value delayed Pension Increases for members. Leave
this box unchecked if Pension Increases are payable from retirement.

This field is only available to some users.

## Age Increases Commence

If [Delayed Increase in Payment](#actives_basis+delayedpi) is
checked, enter the age pension increases will commence from. This field
only applies to Retirement Benefits (and not ill-health benefits).

For example, assume a pension of £100 is paid at age 65. If pension
increases had been granted the pension at 70 would be £130. The Age
Increases Commence is set to 70. The pension valued between age 65 and
70 will be £100. The pension valued at age 70 including the pension
increases that would have been paid between age 65 and 70 will be £130.
The pension from age 70 will increase in line with the pension increases
specified.

The pension cashflows (before applying probabilities), between age 65
and 70 would be £100 pa. From age 70 onwards, the pension cashflows
would be £130 pa, increasing in future years by the pension increases
assumption.

This field is only available to some users.

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