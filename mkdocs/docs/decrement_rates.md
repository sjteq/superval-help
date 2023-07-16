# Decrement Rates



## Retirement Rates

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

## Actives Ill-Health Retirement Rates

This field is used to define the ill-health retirement decrement at each
age. All decrement rates entered are assumed to be independent. SuperVal
will derive the dependent rates from these.

Double click to select from either an age related retirement table (`I`
type) or an age and service related table (`IM` type). The service start
date used to calculate the duration of service when applying `IM` type
tables can be varied using the [Date for Durational
Decrements](actives_basis+durndate.md) field. To ignore ill health
retirement select the table `I000` which contains zeros at all ages.

The ill-health decrement is always assumed to take place half-way
through the year.

Note: Not all options are available to all users.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Actives Leaving Service Rates

This field is used to define the withdrawal from active service
decrement at each age. All decrement rates entered are assumed to be
independent. SuperVal will derive the dependent rates from these.

Double click to select from either an age related withdrawal decrement
table (`L` type) or an age and service related table (`LM` type). The
service start date used to calculate the duration of service when
applying `LM` type tables can be varied using the [Date for Durational
Decrements](actives_basis+durndate.md) field. To ignore withdrawal from
active service select the table `L000` which contains zero at all ages.

Note that a `LM` table should have rates entered for all durations of
service i.e. if defining a select withdrawal rate tables then this should
also have the ultimate rates entered for all future years of service.

The withdrawal decrement is always assumed to take place half-way
through the year.

As an alternative to using `LM` type tables the `L` type tables can be
weighted by duration of service using the Duration Weighting fields.

Note: Not all functionality is available to all users.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Durational Weights

This field can be used to approximate select withdrawal rates. Double
click to select the table containing the multiplier to apply at each
duration. The duration will be calculated as the period from the
member’s Date Joined Company.

For example, a duration related table with `2` at term 0 and `1`
elsewhere would mean that the age-related withdrawal decrement was
doubled for the first year of Company service but normal thereafter.

To specify a withdrawal decrement that relates only to duration, set the
age-related withdrawal decrement to table `W001` (i.e. 1 at all ages) and
enter the decrements here.

If you do not wish to adjust for duration select the table `T000` here.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Transfers Out Rates

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

## Proportion of Retirees Transferring Out

This field is used to define the proportion of retirees who are transferring out at each retirement age.

Double-click to select from an age-related transfer table (`TP` type).
To ignore transfers out at retirement, select the table `TP000 `which contains zero at all ages. 
The table description will be shown to the right of this field.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

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