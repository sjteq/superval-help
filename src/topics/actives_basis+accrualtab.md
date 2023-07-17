# Accrual Rate Table

If the accrual rate varies by age or service then this field can be used
instead of [Accrual Rate](actives_basis+accrate.md) or the [Accrual
Rate Data Item](actives_basis+accrate.md).

## Accrual varies by duration of service

If the accrual rate varies by service, then the table entered is indexed
by the service period defined on the Benefit Slice. Double click to
select an `HT` type table that contains the cumulative Accrual Rate
Table. (Note the service defined on the slice is only used to reference
the table and not in the Benefit Calculations.) For example, if the
accrual rate was 80ths for the first 10 years service and then 60ths
thereafter, the table would have 0.1250 at duration 10 (10 &times; 1/80) and
0.1417 at duration 11 (10/80 + 1/60).

## Accrual Varies by age

If the accrual rate varies by age, then the table entered is indexed by
the member’s age. Double click to select an `HX` type table that
contains the Accrual Rate for each age. The rate at the members age will
then be multiplied by the service period defined for the Benefit Slice.
For example, if the accrual rate was 80ths before age 40 and 60ths
thereafter, the table would hold the value 0.0125 at each age below 40
and 0.0167 at each age above 40.

Please note that the Accrual Rate Table can only be applied to service
in a single Slice and cannot be applied *across* Benefit Slices (or
Tiers). To value different Accrual Rates across different Slices then
consider using the [Service Related Accrual
Table](actives_basis+sratab.md).

Some functionality only available to some users.
