# Pensioners Basis: Spouse



## Spouse Parameter Set

Spouse Parameter Set is a Scheme Global parameter which groups the
Spouse variables. This can be created by using either the `Create
Globals` function or using the _Add/Edit Spouse Parameters_ button. Once
created, these parameters can be edited without going back into the
Basis similar to other global parameter sets.

## Spouse Definition

Select from the drop-down list how to value the spouse’s pension on
death after retirement. The options are:

-   Retirement
-   Death

If Retirement is selected, SuperVal will use the proportion married as
at the member’s age at retirement.

If Death is selected, SuperVal will use the proportion married as at the
member’s age at death.

For more information please see the Infocus Document relating to
Proportion Married.

## Ignore Spouse Details in Data (Marital Status/Spouse Date of Birth)

Ignore the spouse data provided in the member data

## Male Proportion Married Table

## Female Proportion Married Table

Double click to select the table containing the proportion married for
members at each age.

In ongoing runs, these fields are used to determine the proportion of
the member’s benefit paid to a spouse or partner on death in service
(actives only), death in deferment or death after retirement. The field
[Spouse’s Definition](#bases+spmethod) enables you to select how the
proportion married is applied.

In PPF runs the fields in the Scheme PPF parameters can be used to enter
the proportion married separately for male and female spouses and male
and female partners.

If 90% of members are assumed to be married at all ages then enter a
table containing `0.9`.

More information is available in the Infocus Document called Proportion
Married.

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

## Male Proportion Married

## Female Proportion Married

Users can express the proportion married as a single percentage across all ages.

## Male Age Difference Table (m-f)

## Female Age Difference Table (f-m)

This field is used to enter an age-dependent table if the age difference
between a member and their spouse varies according to the member’s age.
It is used when valuing death benefits prior to retirement and
contingent annuities on death after retirement. For pensioners death
benefits prior to retirement may occur when the [Benefit Commencing
Age](pensioners_basis+bage.md) is after the member’s current age.

Double click to select the `AD` table that contains the relevant data.
The table should contain the values for Member’s Age minus Spouse’s Age
ie if Members are 3 years older than their spouse enter `3`.

This field is only available to some users.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Male Age Difference (m-f)

## Female Age Difference (f-m)

This field is used to set an age difference between a member and their
spouse that is identical for all members. It is used when valuing death
benefits prior to retirement and contingent annuities on death after
retirement. For pensioners death benefits prior to retirement may occur
when the [Benefit Commencing Age](pensioners_basis+bage.md) is after
the member’s current age.

Enter the relevant value containing Member’s Age minus Spouse’s Age ie
if Members are 3 years older than their spouse enter `3`.

If you wish to use an Age Rating that varies with the member’s age then
leave this field blank and the Age Difference Table will become
available. (This functionality is not available for PPF runs or for the
annuity calculators.)

The Age Difference Table field is only available to some users.

## Project "Unknown" Spouse from Retirement

Indicate if `unknown` Spouse (Marital Status other than M, S or W) is to
be projected from Retirement (using Proportion Married/Age Difference at
Retirement and Spouse Mortality since then)

## Retirement Date for "Unknown" Spouse

Specify the Retirement Date to be used for project Spouse

Please see Release Note V9.20 for details

## Retirement Age for "Unknown"Spouse

Specify the Retirement Age to be used for projects spouse

## Add/Edit Spouse Parameters

Add or Edit any Spouse parameter sets.

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