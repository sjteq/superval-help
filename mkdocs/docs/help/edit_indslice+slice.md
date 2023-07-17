# Edit IndSlice: Slice



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

## Start Date

## Earliest Start Date

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

## Finish Date

## Latest Finish Date

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

## Male Payment Start Age

## Female Payment Start Age

When valuing Independent Slices, the user can choose a start age for the
payment of the benefit.

To value a cash benefit, the Payment Start Age should be equal to the
[Payment End Age](#actives_basis+payend).

## Male Payment End Age

## Female Payment End Age

When valuing Independent Slices, the user can choose a end age for the
payment of the benefit.

To value a cash benefit, the [Payment Start
Age](#actives_basis+paystart) should be equal to the Payment End Age.

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

## Pension Increases Pre Start

This field is used to set a pension increase that will apply from the
date the member retires (where this is before Payment Start Age) and the
Payment Start Age. Select from the drop-down list the appropriate rate.
The options are:

-   Main Pension
-   Special Pension
-   Pension Increase 3
-   Pension Increase 4

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
Pension](actives_basis+fixpen.md) in Tiers 1, 2 or 3.

## ERF Tables

## ERF/LRF Tables

Select from the drop-down list which of the Early/Late Retirement Factor
Tables to apply to the benefit arising from this Benefit Slice. (The
Early-Retirement Factors are defined on the Ret Pension Tab. The Late
Retirement Factors are defined on the Late Retirement Tab.) The options
are as follows:

-   ERF1/LRF1 (Revaln 1 + 3) or ERF1/LRF1 (Revaln 2)
-   ERF2/LRF2 (Revaln 1 + 3) or ERF2/LRF2 (Revaln 2)

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

## Previous Ind. Slice

Move back to the previous Independent Slice. Select "ok" to save any changes to the current Independent Slice.

## Next Ind. Slice

Move on to the next Independent Slice. Select "ok" to save any changes to the current Independent Slice.

## OK

When you have finished entering the relevant information, click the _OK_
button to move to the next screen.

SuperVal will check that all of the required entries on the page have
been made. If additional fields require data SuperVal will show briefly
in red which is the first of these fields found on the page.

## Cancel

Clicking on the _Cancel_ button allows you to return to the previous
screen without saving any of your changes.