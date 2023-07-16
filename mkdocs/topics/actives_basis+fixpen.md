# Pension Data Item

Select from the drop-down list the data item containing the Fixed
Pension Amount. This might have arisen from either a transfer-in or a
past service CARE benefit.

## Increase in Service

If the Benefit Basis is CARE, then this pension amount will be increased
in service at the [CARE Revaluation Rate](actives_basis+salrev.md).

If the Benefit Basis is Final Salary, then this pension amount will not
be increased in service. (To value a fixed pension that increases in
line with salaries, instead consider defining a salary equal to the
pension amount and setting up a Slice with an accrual rate of 1/1
multiplied one year of service.

## Increase in Deferment

This pension amount will be increased in deferment at the [Revaluation
in Deferment](actives_basis+revdefind.md) Rate specified on the Slices
Tab. (The rate chosen will impact on the Early-Retirement Factors that
are used.)

Note: A Pension Data Item and benefit accrual can be specified in the
same Slice as long as they are on different Tiers. Alternatively they
can be specified on different Slices.
