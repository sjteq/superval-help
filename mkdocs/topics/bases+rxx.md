# Early/Late Retirement Decrement Table

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
