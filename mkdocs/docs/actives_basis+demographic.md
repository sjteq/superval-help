# Actives Basis: Demographic



## Male Decrement Rates  Parameter Set

## Female Decrement Rates  Parameter Set

Decrement Rates Parameter set is a Scheme Global parameter which groups
the Male or Female Decrement variables. This can be created by using
either the `Create Globals` function or using the _Add/Edit Decrement
Rates_ button. Once created, these parameters can be edited without
going back into the Basis similar to other global parameter sets.

## Male Retirement Rates

## Male Early/Late Retirement Rates

## Female Retirement Rates

## Female Early/Late Retirement Rates

This field is used to define the early/late retirement decrement rate at
each age. All decrement rates entered are assumed to be independent.
SuperVal will derive the dependent rates from these.

## Actives 

Double click to select from either an age related retirement
table (`R` type) or an age and service related retirement table (`RM`
type). The service start date used to calculate the duration of service
when applying `RM` type tables can be varied using the [Date for
Durational Decrements](#actives_basis+durndate) field. To ignore
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

## Male Ill-Health Retirement Rates

## Female Ill-Health Retirement Rates

This field is used to define the ill-health retirement decrement at each
age. All decrement rates entered are assumed to be independent. SuperVal
will derive the dependent rates from these.

Double click to select from either an age related retirement table (`I`
type) or an age and service related table (`IM` type). The service start
date used to calculate the duration of service when applying `IM` type
tables can be varied using the [Date for Durational
Decrements](#actives_basis+durndate) field. To ignore ill health
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

## Male Leaving Service Rates

## Female Leaving Service Rates

This field is used to define the withdrawal from active service
decrement at each age. All decrement rates entered are assumed to be
independent. SuperVal will derive the dependent rates from these.

Double click to select from either an age related withdrawal decrement
table (`L` type) or an age and service related table (`LM` type). The
service start date used to calculate the duration of service when
applying `LM` type tables can be varied using the [Date for Durational
Decrements](#actives_basis+durndate) field. To ignore withdrawal from
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

## Male Durational Weights

## Female Durational Weights

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

## Date for Durational Decrements/Salary Scale

If using durational decrements (age &times; service related decrements) or a
service related promotional scale, then select from the drop-down list
the date to use as the member’s service start date. The duration of the
decrement at the point of exit or the promotional salary scale to apply
will be based on service from this date.

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

## Add/Edit Decrement Rates

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