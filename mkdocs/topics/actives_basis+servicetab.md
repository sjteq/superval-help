# Accelerated Service Table

If the service granted for each year of accrual is greater than actual
service then this field can be used to determine the service credit.
Double click to select an `ET` type table containing the cumulative
service credit that will be indexed by the period of service defined on
the Benefit Slice. The corresponding value in the ET table will be used
in the Benefit Calculations. (Part years will be linearly interpolated.)

For example, a member receives an additional 5 years pensionable service
on completion of 10 years. The `ET` table would have an entry of `9` at
duration 9 and `15` at duration 10, `16` at 11 etc.

The Accelerated Service Table should not be used with a maximum service
restriction but instead the maximum service should be contained within
the Table used.

Please note that the Accelerated Service Table can only be applied to
service in a single Slice and cannot be applied _across_ Benefit Slices
(or Tiers). To value different Accrual Rates across different Slices
then consider using the [Service Related Accrual
Table](actives_basis+sratab.md).

Some functionality is only available to some users.
