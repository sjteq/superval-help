# Accrual Rate or Accrual Rate Date Item

Enter both the numerator and the denominator for the rate of accrual
where this is the same for all members for this Benefit Slice i.e. for
1/60th accrual enter `1` in the numerator and `60` in the denominator.

If the accrual rate varies by member, then leave these two fields blank
and this will enable you to enter an Accrual Rate Data Item instead.
Select from the drop-down list the data item containing the Member
Specific Accrual Rate. The data item should contain the Accrual Rate as
a percentage i.e. for 1/60th use `0.01667`. (This might be used when each
member has a targeted benefit of 2/3rds over their career but receive a
pro-rata amount on earlier exit. The Member Specific Accrual Rate
Calculator can be used to calculate such a data item.)

The benefit from the Tier will be calculated as the accrual rate
(numerator/denominator) times [Salary](actives_basis+salcod.md) times
service. The service would be the period specified on the Benefit Slice,
or [Accelerated Service Table](actives_basis+servicetab.md), or [Added
Years](actives_basis+addyrs.md).

When using [Accelerated Service Tables](actives_basis+servicetab.md) or
[Service Related Accrual Tables](actives_basis+sratab.md), enter the
underlying Accrual Rate that applies to all service here. Either the
Accelerated Service Table or the Service Related Accrual Table will
contain the number of years of the underlying Accrual Rate at each
duration.

To enter a Fixed Pension, ensure both these and the
[Salary](actives_basis+salcod.md) field above are blank.
