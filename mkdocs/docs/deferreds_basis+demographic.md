# Deferreds Basis: Demographic



## Male Decrement Rates  Parameter Set

## Female Decrement Rates  Parameter Set

Decrement Rates Parameter set is a Scheme Global parameter which groups
the Male or Female Decrement variables. This can be created by using
either the `Create Globals` function or using the _Add/Edit Decrement
Rates_ button. Once created, these parameters can be edited without
going back into the Basis similar to other global parameter sets.

## Male Retirement Rates

## Female Retirement Rates

This field is used to define the early/late retirement decrement rate at
each age. All decrement rates entered are assumed to be independent.
SuperVal will derive the dependent rates from these.

## Actives 

Double click to select from either an age related retirement
table (`R` type) or an age and service related retirement table (`RM`
type). The service start date used to calculate the duration of service
when applying `RM` type tables can be varied using the [Date for
Durational Decrements](actives_basis+durndate.md) field. To ignore
early/late retirement select the table `R000 `which contains zero at all
ages. The table description will be shown to the right of this field.

Members who retire prior to NRA are assumed to retire half-way through
the year. Members who retire at NRA or after are assumed to retire on
the anniversary of the valuation date.

On reaching the NRA (or LRA if later) specified in the basis file,
SuperVal will retire all members regardless of any entry in this table.
Members who are over NRA (or LRA if later) at date of valuation will be
assumed to retire immediately.


## Deferreds

For deferred members, double click to select an age
related retirement table (`R` type). To ignore early retirement select
the table `R000 `which contains zero at all ages. The table description
will be shown to the right of this field.

On reaching the NRA specified in the basis file, SuperVal will retire
all members regardless of any entry in this table. Members who are over
NRA at date of valuation will be assumed to retire immediately.

Note: The Late Retirement functionality is only available to some users.

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

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Male Transfers Out Rates

## Female Transfers Out Rates

This field is used to define the transfer-out decrement rate at each age (non-retirement ages). 
Decrement rates entered are assumed to be independent.
SuperVal will derive the dependent rates from these.

Double-click to select from an age-related transfer table (`TO` type).
To ignore transfers out, select the table `TO000 `which contains zero at all ages. 
The table description will be shown to the right of this field.

Members who transfer out are assumed to exit half-way through the year.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Proportion of Male Retirees Transferring Out

## Proportion of Female Retirees Transferring Out

This field is used to define the proportion of retirees who are transferring out at each retirement age.

Double-click to select from an age-related transfer table (`TP` type).
To ignore transfers out at retirement, select the table `TP000 `which contains zero at all ages. 
The table description will be shown to the right of this field.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Add/Edit Decrement Rates

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