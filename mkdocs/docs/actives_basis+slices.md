# Actives Basis: Slices



## Slice Description

Up to 16 separate Benefit Slices can be specified. Slice 1 will always
be used to describe future service. Slices 2 to 16 are used to describe
past service.

Enter a description for the Benefit Slice being valued eg Pre Barber
Benefit.

This description will appear on the results output.

The Alt Slices Tab will only be available if you have selected an option
other than Ignore in the [Alternate Slices
Method](actives_basis+altsw.md) field on the Main Tab.

The Ind Slices Tab will only be available if you have checked the box
for [Independent Slices](actives_basis+indslices.md) on the Main Tab.

## Start Date [Data Item]

## Earliest Start Date [Fixed Date]

The Service Start Date for each Slice is entered here. Select from the
drop-down list the data item containing the relevant data item. This
will be used as the date when service for this Slice starts accruing
unless an Earliest Start Date is also defined.

The user can define the Earliest Start Date that can be used for a
particular Slice. Enter this date in the following date format
DD/MM/CCYY. SuperVal will then take the later of these two dates to
determine when service for this Slice starts accruing.

If valuing future service, the Service Start Date on Slice 1 should be
`Valuation Date` and the Earliest Start Date should be blank. If you
have no future service liabilities, please ensure these fields are left
blank on Slice 1.

If the Slice is being used to value added years or a fixed pension then
these field can be left blank.

The Earliest Start Date will not be used for future service benefits on
Slice 1 when CARE benefits are being valued.

## Finish Date [Data Item]

## Latest Finish Date [Fixed Date]

The Service Finish Date for each slice is entered here. Select from the
drop-down list the data item containing the relevant data item. This
will be used as the date when service for this Slice stops accruing
unless a Latest Finish Date is also defined.

The user can define the Latest Finish Date that can be used for a
particular Slice. Enter this date in the following date format
DD/MM/CCYY. SuperVal will then take the earlier of these two dates to
determine when service for this Slice stops accruing.

If valuing future service, the Service Finish Date on Slice 1 will
always be `Leaving Date`. The Latest Finish Date could be used to cease
accrual at a fixed date in the future. If you have no future service
liabilities, please ensure these fields are left blank on Slice 1. The
Latest Finish Date will not be used for future service benefits on Slice
1 when CARE benefits are being valued.

If the Slice is being used to value added years or a fixed pension then
these field can be left blank.

The Latest Finish Date on the [Offset Slice](actives_basis+sliceup.md)
must be specified as this is used to identify the date at which GMPs
stopped accruing, for some Cash Commutation or death in deferment
options.

## Service Rounding Override

The Company Service and Scheme Membership used by SuperVal can be
rounded in a number of different ways. Select from the drop-down list
one of the following options:

-   Exact Days
-   Months Rounded Down
-   Nearer Months
-   Months Rounded Up
-   Years Rounded Down
-   Nearer Years
-   Years Rounded Up
-   Complete Tax Years

The entry on the Membership Tab will be used unless an Override is
specified on a particular Slice. Note, service is rounded on a Slice by
Slice basis and there is no rounding for total service.

## Added Years

This field is used to define the number of Added Years either where
these are fixed for all members or a member specific amount. To enable
it ensure the [Start Date](#actives_basis+stdate) for this slice is
blank. Added Years might have arisen from an Augmentation exercise or a
Transfer-In to the scheme.

If the number of Added Years granted is the same for all members, enter
the number of years granted in years (and part) years i.e. for 5 years and
6 months enter `5.5`.

If the number of years varies per member, then select from the drop-down
list the data item containing the appropriate data. The data item should
contain the number of complete (and part) years granted to each member.

## Count Towards Maximum Service

The maximum amount of service at retirement is defined in the
[Retirement Maximum Service/Retirement Maximum Service
Table](actives_basis+srvmax.md) field on the Membership Tab. On each
Slice you can choose whether the service from that Slice should be
included when comparing total service to the Maximum Service. Check this
box if service from this Slice should be included. Leave the box
unchecked if service from this Slice should not be included in the
comparison.

SuperVal will limit the benefits if the total service from all of the
Slices where this box is checked exceeds the Maximum Service specified
on the Membership Tab. The service will be restricted at the point that
it exceeds the maximum i.e. SuperVal will start at the largest Slice
Number on which benefits are defined and work down to Slice 1 (the
future service Slice). The benefits on the Slice where the Maximum
Service is exceeded will be reduced. All Slices with a lower number will
have a zero liability.

## Revaluation in Deferment

This is the rate at which the benefits from this Slice will increases in
deferment i.e. between date of leaving active service and NRA.

Select from the drop-down list which of the 3 revaluation rates
previously defined should be used. The options are:

-   Rate 1
-   Rate 2
-   Rate 3

The rate entered will be applied to all types of benefit entered ie
normal accrual, added years and a pension data item.

The values of these three deferred revaluation rates are entered on the
Financial Tab.

## Pension Increases in Payment

Once in payment, the pension from this Slice or PUP, can be set to
increase at one of four different increase rates. Select from the
drop-down list the appropriate rate. The options are:

-   Main Pension
-   Special Pension
-   Pension Increase 3
-   Pension Increase 4

## Count Towards IR Maximum

Any Inland Revenue Limits to apply are defined by the IR Maximum
Parameters on the Legislation Tab. Check this box if the benefit from
this Slice should be included in the comparison against the IR maximum
benefit. Leave this box unchecked if the benefits from this Slice should
not be included in the comparison against the IR maximum benefit.

## Include In Underpin

Any Underpin to apply is defined by the Underpin Contribution Parameters
on the Contributions Tab. Check this box if the benefit from this Slice
should be included in the comparison against the Underpin benefit. Leave
this box unchecked if the benefits from this Slice should not be
included in the comparison against the Underpin benefit.

## Benefit Basis

Select from the drop-down list whether the benefits described on this
Slice are a Final Salary benefit or Career Average Revalued Earnings
(CARE) benefit.

If Final Salary is selected then the benefit calculated from this Slice
will increase in line with salary increases until retirement or earlier
exit. The salary increase used will be taken from the [Salary Increase
Rate](actives_basis+salinc.md) on the Financial Tab unless this has
been overridden by the [Salary Increase
Override](actives_basis+salinf.md) field on the Salary Tab.

If CARE is selected then the benefit calculated from this Slice will
increase in line with the [CARE Revaluation
Rate](actives_basis+salrev.md) on the Financial tab. Note that for past
service CARE Slices the pension amount as at the Valuation Date is
needed and should be entered as a [Fixed
Pension](#actives_basis+fixpen) in Tiers 1, 2 or 3.

## ERF Tables

## ERF/LRF Tables

Select from the drop-down list which of the Early/Late Retirement Factor
Tables to apply to the benefit arising from this Benefit Slice. (The
Early-Retirement Factors are defined on the Ret Pension Tab. The Late
Retirement Factors are defined on the Late Retirement Tab.) The options
are as follows:

-   ERF1/LRF1 (Revaln 1 + 3) or ERF1/LRF1 (Revaln 2)
-   ERF2/LRF2 (Revaln 1 + 3) or ERF2/LRF2 (Revaln 2)

## Ignore for CARE Prospective

Check this box if the benefits described on this Benefit Slice should be
excluded from the prospective CARE benefits. Leave this box unchecked if
the benefits should be included.

## Spouse's DAR Override

The user has the option to enter an override for the [Spouse’s Death
after Retirement Percentage](bases+warfrac.md) entered on the Ret
Pension Tab.

Either enter the fixed percentage override as a percentage i.e. for 50%
enter `50` rather than `0.5`.

If you do not wish to use this option then leave blank.

## Tier 2 Benefits Defined

## Tier 3 Benefits Defined

Check the Tier 2 Benefits Defined box if you wish to define a second
Tier of benefits. Leave unchecked if there is no additional Tier of
benefits. If checked, the user will have the option to check the Tier 3
Benefits Defined Box to define a third Tier of benefits.

The benefits defined on either the second or third Tier can be added.
Alternatively, the user has the option to subtracted a previous Tier
from the final Tier of benefits defined i.e. Tier 1 or the sum of Tier 1
and Tier 2 can be deducted from Tier 3, or Tier 1 can be deducted from
Tier 2.

## Male PPF NRA (Levy Valuations)

## Female PPF NRA (Levy Valuations)

On the Legislation Tab, enter the NRA to be attached to the GMP, which
is converted in to excess pension, for PPF valuations.

Elsewhere, for Actives and Deferreds, select from the drop-down list
which of the previously defined PPF NRAs applies to the pension or
benefit slice. The PPF NRAs are specified on the PPF/Cap Tab.

For Pensioners enter the normal retirement age to be used as the PPF NRA
in the PPF (S179 Levy) Valuation. The PPF NRAs are only used to
determine the level of capping required. They do not override the
Benefit Commencing Age. To allow for ill health retirements, use a
sufficiently low age so that all members exceed this age i.e. 16. To allow
for early retirement pensions, use an age such as 50.

## PPF Service Period

PPF guidance, requires the user to show separately the Pre-1997 pension,
post 6 April 1997 to 5 April 2009 pension and the Post 6 April 2009
pension.

Select from the drop-down list whether the pension is:

-   Pre-97
-   97 to 09
-   Post-09

## Salary

Select from the drop-down list which of the salaries defined on the
Salary Tab to use in the calculation of benefits from this Tier/Slice.

Leave this field blank to enable the [Fixed
Pension](#actives_basis+fixpen) field where a fixed pension benefit
can be valued.

## Accrual Rate Multiplier

## Accrual Rate Divisor

## Accrual Rate [Data Item]

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
Years](#actives_basis+addyrs).

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

## Fixed Pension [Data Item]

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
in Deferment](#actives_basis+revdefind) Rate specified on the Slices
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

## Grid Help

Right-clicking on a Row Number presents a menu with the following
options, which allow you to expand or reduce the number of rows of data
to be entered:

-   Add a New Row to the bottom of the grid;
-   Insert a New Row at the position of the cursor; and
-   Delete the Current Row at the position of the cursor.

## Grid Help

Right-clicking on the Top Left Corner of the grid displays a menu which
allows you to set the following Grid Editing Options:

-   Editing of a cell can be invoked by either clicking on the cell or
    by pressing F2 when the cell is active (Clicking will only change
    the current active cell); and
-   determine the cursor movement once editing is complete to be either
    to the next cell down, the next cell to the right or to stay in the
    current cell.

## Add Slice

Clicking on the _Add Slice_ button allows you to add another Slice of
benefits. Select from the box which of the slices the benefits on the
new Slice should be based on. The choices are `Default` (to base the Slice
on the defaults specified) or one of the existing Slices to copy an
existing slice of benefits. The Slice will always be added at the end of
current Slices.

## Insert Slice

Clicking on the _Insert Slice_ button allows you to insert another Slice
definition. Select from the list of slices the slice definition you want
to insert the new slice before.

## Edit Slice

Pressing the _Edit Slice_ button allows you to edit a Slice definition.
You must select the Slice definition to be edited, unless a Slice
definition is currently highlighted, in which case this Slice definition
will be edited.

## Delete Slice

Pressing the _Delete Slice_ button allows you to, after confirmation,
delete a Slice definition. You must select the Slice definition to be
deleted, unless a Slice definition is currently highlighted, in which
case this Slice definition will be deleted.

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