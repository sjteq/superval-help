# Withdrawal Decrement Table

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
