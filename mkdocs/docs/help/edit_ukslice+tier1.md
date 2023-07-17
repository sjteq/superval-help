# Edit UKSlice: Tier1



## Salary

Select from the drop-down list which of the salaries defined on the
Salary Tab to use in the calculation of benefits from this Tier/Slice.

Leave this field blank to enable the [Fixed
Pension](#actives_basis+fixpen) field where a fixed pension benefit
can be valued.

## Accrual Rate

## Accrual Rate Data Item

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
(numerator/denominator) times [Salary](#actives_basis+salcod) times
service. The service would be the period specified on the Benefit Slice,
or [Accelerated Service Table](#actives_basis+servicetab), or [Added
Years](actives_basis+addyrs.md).

When using [Accelerated Service Tables](#actives_basis+servicetab) or
[Service Related Accrual Tables](#actives_basis+sratab), enter the
underlying Accrual Rate that applies to all service here. Either the
Accelerated Service Table or the Service Related Accrual Table will
contain the number of years of the underlying Accrual Rate at each
duration.

To enter a Fixed Pension, ensure both these and the
[Salary](#actives_basis+salcod) field above are blank.

## Accrual Rate Table

If the accrual rate varies by age or service then this field can be used
instead of [Accrual Rate](#actives_basis+accrate) or the [Accrual
Rate Data Item](#actives_basis+accrate).

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
Table](#actives_basis+sratab).

Some functionality only available to some users.

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

## Accelerated Service Table

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
Table](#actives_basis+sratab).

Some functionality is only available to some users.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Service Related Accrual Table

This is `ET`, `FT`, `GT` and `HT` type rate tables, which is indexed by
the period of service specified by the Benefit Slice. It is the
corresponding entry on the `ET`, `FT`, `GT` and `HT` table that is used
in the benefit calculation.

The service period is calculated from [DOE Qualifying
Service](actives_basis+doeqs.md) to the start date/end date on the
slice. SuperVal will then linearly interpolate to obtain the value for
the member’s exact period of service.

Typical uses for this table may be uplifted service or extra years of
service granted after a certain period. For example, suppose that
members receive a further 5 years pensionable service on completion of
10 years. The Service Related Accrual Table would have an entry of `9` at
duration 9 and `15` at duration 10, `16` at 11 etc. i.e. the table is
cumulative.

Please note that the Service Related Accrual Table will be applied
across Benefit Slices (or Tiers).

If a `ET`, `FT`, `GT` and `HT` table is not defined, then the service
will be the period between the Start Date (or minimum start date) and
Finish Date (or maximum finish date) for the Benefit Slice. Allowance
would be made for maximum service.

Double click to select from the list of available `ET`, `FT`, `GT` and
`HT` type rate tables.

When using this field, you will be required to enter the date from which
service starts to accrue in the [DOE Qualifying
Service](actives_basis+doeqs.md) on the Membership Tab.

Not all functionality is available to all users.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Fixed Pension

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

## Minimum Pension

This field can be used to define a minimum amount of pension that will
be provided from this Tier of the particular Slice. This can either be
fixed for all members of be member specific. Either enter the amount of
the minimum pension or select from the drop-down list the data item
containing the member specific data. The amount entered will not be
increased by SuperVal between the valuation date and the point of exit
ie retirement, withdrawal, death.

If no minimum applies then leave this field blank.

## Maximum Pension

This field can be used to define a maximum amount of pension that that
will be provided from this Tier of the particular Slice. This can either
be fixed for all members of be member specific. Either enter the amount
of the maximum pension or select from the drop-down list the data item
containing the member specific data. The amount entered will not be
increased by SuperVal between the valuation date and the point of exit
ie retirement, withdrawal or death.

If no maximum applies then leave this field blank.

## Pension Adjustment Factor

A negative or positive loading can be applied to the pension calculated
from this Tier of benefits. This loading can either be fixed for all
members or be a member specific amount.

For a fixed adjustment, enter the number as a multiplier i.e. `1.1` for a
10% increase or `0.9` for a 10% decrease. If no adjustment is required
enter `1`. If `0` is entered the liability for this Tier will be zero. To
value a negative pension based on the parameters on the Tier, enter `-1`.

For a member specific adjustment, select from the drop-down list the
data item containing the member specific adjustment factor.

The pension calculated in this Tier will be multiplied by the data item
entered in this field.

## Deduct Tier 1

## Deduct Tier 2

You can deduct the benefits calculated on Tier 1 from either of the
benefit calculated on Tier 2 or Tier 3. In Tier 3 you can also deduct
the sum of benefits calculated in Tiers 1 and 2. Check these boxes to
determine which of the Tiers are deducted.

Typical use of this field is for a greater-of benefit comparison. For
example, suppose a scheme provides a benefit which is the greater of
$\frac{Service \times Salary}{80}$ and $\frac{Service \times (Salary - LEL)}{60}$.

Two salaries have been defined in the Salary Tab i.e. `Salary1` is Salary
with no deduction and `Salary2` is Salary with a LEL deduction.

The benefits on Tier 1 will be set up to define the 1/80ths benefit. The
benefits on Tier 2 will be set up to define the excess of the 1/60th
benefit over the 1/80th benefit where this is greater than 0. Specify
the 1/60th benefit on Tier 2 then check the box to deduct Tier 1. Also
ensure that the Minimum Pension specified is zero. (This will ensure the
excess is only valued where greater than zero.) The total benefit valued
by the Tiers will be:

1/80ths + Max (1/60ths – 1/80ths, 0) multiplied by the respective
salaries and service.

## Male PPF Adjustment Factor

## Female PPF Adjustment Factor

A negative or positive loading can be applied to the pension calculated
from this Tier of benefits on a PPF valuation. This loading can either
be fixed for all members or be a member specific amount.

For a fixed adjustment, enter the number as a multiplier i.e. `1.1` for a
10% increase or `0.9` for a 10% decrease. If no adjustment is required
enter `1`. If `0` is entered the liability for this Tier will be zero. To
value a negative pension based on the parameters on the Tier, enter `-1`.

For a member specific adjustment, select from the drop-down list the
data item containing the member specific adjustment factor.

The pension calculated in this Tier will be multiplied by the data item
entered in this field.

## Previous Slice

Move back to the previous Slice. Select "ok" to save any changes to the current Slice.

## Next Slice

Move on to the next Slice. Select "ok" to save any changes to the current Slice.

## OK

When you have finished entering the relevant information, click the _OK_
button to move to the next screen.

SuperVal will check that all of the required entries on the page have
been made. If additional fields require data SuperVal will show briefly
in red which is the first of these fields found on the page.

## Cancel

Clicking on the _Cancel_ button allows you to return to the previous
screen without saving any of your changes.