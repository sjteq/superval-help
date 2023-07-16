# Death in Deferment Pension: Benefit Basis

Select from the drop-down list how the spouse’s death in deferment
pension benefits should be defined. The options are:

-   None
-   GMP then Spouse’s Fraction
-   GMP then 1/160 Revalued
-   Max(GMP,1/160) then Spouse’s Fraction
-   Max(GMP,1/160) then 1/160 Revalued
-   Spouse’s Fraction

For options other than `None` or `Spouse’s Fraction` the benefits will
be calculated differently for Slices before and after the [Offset
Slices](actives_basis+sliceup.md) (the lowest slice number for which
GMPs underlying the benefits).

Consider the following service time line:

![](img/bm9.gif)

The benefit for each option in each of the periods is as follows:

Option | Offset Past Service | Rest Past Service | Future Service
-------|---------------------|-------------------|---------------
None | None | None | None
GMP then Spouse’s Fraction | Spouse’s GMP | % of Member’s Pension | % of Member’s Pension
GMP then 1/160 Revalued | Spouse’s GMP | 1/160 &times; Salary &times; Service, revalued in deferment | 1/160 &times; Salary &times; Service, revalued in deferment
Max (GMP,1/160) then Spouse’s Fraction | Greater of: Spouse’s GMP and 1/160 &times; Salary &times; Service | % of Member’s Pension | % of Member’s Pension
Max (GMP,1/160) then 1/160 Revalued | Greater of: Spouse’s GMP and 1/160 &times; Salary &times; Service | 1/160 &times; Salary &times; Service, revalued in deferment | 1/160 &times; Salary &times; Service, revalued in deferment
Spouse’s Fraction | % of Member’s Pension | % of Member’s Pension | % of Member’s Pension


Please note the following about the above benefits:

## GMP then 1/160 Revalued Benefit

The Start Date for the 1/160th benefit will be later of the [Not After
Date](actives_basis+fndate.md) that is specified on the [Offset
Slice](actives_basis+sliceup.md) and the [Start
Date](actives_basis+diddat.md) specified on this Tab.

The Finish Date for the 1/160th benefit will be the end date of the
lowest number Slice specified i.e. LDATE in Slice 1.

The pension will be revalued in deferment according to the [Deferred
Revaluation Rate](actives_basis+revrat.md) specified on the Financial
tab.

## Max (GMP, 1/160) then Spouse’s Fraction or Max (GMP, 1/160) then 1/160 Revalued

The Start Date for the Max (GMP, 1/160) benefit will be the later of
[Start Date](actives_basis+diddat.md) and [Not Before
Date](actives_basis+diddatmin.md) specified on this Tab. The Finish
Date for the Max (GMP, 1/160) benefit will be the [Not After
Date](actives_basis+fndate.md) that is specified on the [Offset
Slice](actives_basis+sliceup.md).

The Start Date for the 1/160 Revalued in Deferment will be for the [Not
After Date](actives_basis+fndate.md) that is specified on the [Offset
Slice.](actives_basis+sliceup.md) The Finish Date for the 1/160th
benefit will be the end date of the lowest number Slice specified i.e.
LDATE in Slice 1.

For both these options the user will be asked to specify whether to
revalue benefits using the [Revalue Pre-1997
1/160ths.](actives_basis+didrevdef.md) If this box is checked then the
benefit will be revalued according to the [Deferred Revaluation
Rate](actives_basis+revrat.md) specified on the Financial tab .

## Spouse’s Fraction

This will be determined from the benefits described on the Slices
multiplied by the [Benefit Percentage](actives_basis+wdidfrac.md). In
deferment the benefits will be revalued using the rate selected in the
[Revaluation in Deferment](actives_basis+revdefind.md) on the Slices
Tab.

## Note: Added Years and Pension Data Items

When valuing the death in deferment pension any Added Years or Pension
Data Items specified on the Slices are included in the spouse’s death in
deferment benefits valued using the Spouse’s Fraction but not in the
1/160ths pension benefits for death in deferment.
