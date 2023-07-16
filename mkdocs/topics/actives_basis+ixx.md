# Ill Health Decrement Table

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
