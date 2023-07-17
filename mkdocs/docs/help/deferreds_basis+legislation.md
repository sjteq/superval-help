# Deferreds Basis: Legislation



## GMPs as at Leaving Date

Check this box to revalue the member’s GMP between date of leaving and
Date of Valuation.

If checked, the data items loaded for GMP i.e. GMP0 and GMPE0 will be
assumed to be the Pre-1988 GMP and Post-1988 GMP at Date of Leaving
respectively. SuperVal will revalue the GMP to Date of Valuation using
the Fixed Rate Revaluations hard-coded into SuperVal based on the
member’s Date of Exit. The GMP will be revalued using the number of
Tax Years between Date of Leaving and State Pension Age less Tax Years
between Date Of Valuation and State Pension Age. If NRA is greater than
SPA, then Statutory Late Retirement Factors are applied.

If unchecked, SuperVal will assume the data items GMP0 and GMPE0 are the
Pre-1988 GMP and Post-1988 GMP as at Date of Valuation.

SuperVal will revalue the GMP from date of valuation in line with the
information specified on the Legislation tab.

## Fixed Revaluation Rate to SPA

Check this box if the GMP Revaluation Rate to SPA is Fixed.

For Deferreds enter the data item for date of leaving active service in
the [Date Left Active](deferreds_basis+leaving.md) on the Membership
Tab.

If unchecked, the user will be required to enter the rate of revaluation
to use in [Revaluation Rate to SPA](#deferreds_basis+gmprev1).

## Revaluation Rate To SPA

This is the rate at which the GMP will be revalued to SPA when Fixed
Rate Revaluations do not apply.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Past GMP Revaluation Rate(s) to NRA<SPA Factor Set

This field only applies to normal/early retirement pensions before SPA.
It is not used for death in deferment benefits. If GMP retirement
benefits payable before SPA are determined using a different rate of
revaluation to that used to SPA then the past Revaluation Rates should
be entered here.

SuperVal will roll back the GMP at valuation date to GMP as at date of
leaving active service using either [Fixed Revaluation Rate to SPA](#deferreds_basis+gmprev2)
or [Revaluation Rate to SPA](#deferreds_basis+gmprev1) as applicable.
SuperVal will then roll forward the GMP to NRA using the rate(s) specified
here. Therefore, if an entry is made in this field the data item containing
the date of leaving active service must be specified in the [Date Left Active](deferreds_basis+leaving.md)
on the Membership Tab.

Select from the drop-down list the Factor Table Set that contains the
applicable past Revaluation rates.

Note that the Factor Table Set consists of a series of Increase Dates and
Revaluation Rates (%).  The values are NOT cumulative (this differs from
the Factor Table Set currently in use for [Pre Valuation Date Factor Set](deferreds_basis+revset.md)).
Any Increase Dates that fall between a members' Leaving Date and the 
Valuation Date will be included (in full) in the past Revaluation Rates.

## Revaluation Rate to NRA<SPA

This field only applies to normal/early retirement pensions before SPA.
It is not used for death in deferment benefits. If GMP retirement
benefits payable before SPA are determined using a different rate of
revaluation to that used to SPA then that different rate should be
entered here.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

Once selected, the current value of the Global Financial Parameter is
shown to the right of this field.

If this field is left blank, SuperVal will use either [Fixed Revaluation Rate to SPA](#deferreds_basis+gmprev2)
or [Revaluation Rate to SPA](#deferreds_basis+gmprev1) as applicable.

## Complete Years Pre NRA

This field is only available if [Revaluation Rate to NRA&lt;
SPA](#deferreds_basis+presparev) is populated.

Exits before NRA, such as early retirement and death in deferment, are
assumed to occur half-way through the year i.e. 0.5, 1.5, 2.5 years after
the valuation date. By checking this box, the GMP will receive
revaluations for the number of complete years only i.e. 0, 1, 2. If the
box is unchecked, the GMP will receive an additional half-year of
revaluation i.e. 0.5, 1.5, 2.5.

## NRA Exits Rounding

This field is only available if [Revaluation Rate to NRA&lt;
SPA](#deferreds_basis+presparev) is populated. Select from the
drop-down list how the rounding on revaluations of GMP to NRA should be
calculated. The options are:

-   Exact Days
-   Months Rounded Down
-   Nearest Months
-   Months Rounded Up
-   Years Rounded Down
-   Nearest Years
-   Years Rounded Up
-   Complete Tax Years

The discounting of the benefit will be based on years nearest.

## Franking Code

For Actives and Deferred Members, there are five choices for Franking of
GMPs for members retiring before SPA. For Pensioners only the first
three options are available. Select from the drop-down list which of
these to apply. The options are:

-   None
-   Partial Franking
-   Full Franking
-   Maximum Franking
-   No Anti Franking Guarantee

An example to illustrate how these different options work is set out
below:

Suppose you have a male member retiring at 60 with a pension as follows:

-   Pension = £2,000
-   GMP at 60 = £1,000 (included in above figure)
-   GMP at 65 = £1,500

GMP revaluations between 60 and 65 are therefore £500 (£1,500 less
£1,000).

Once in payment, the pension will increase at 5% per annum.

The additional pension at SPA for the GMP revaluations between 60 and 65
under each of the options are as follows:


## None

All of the revaluations on the GMP are added to the pension at SPA.

So, the pension at 65 is calculated as 

$$£2,000 \times 1.05^5 + £500 = £3,053$$


## Partial Franking

Revaluations on the GMP between retirement and SPA, less scheme
increases granted on the GMP, are added to the pension at SPA.

So, the pension at 65 is calculated as 

$$£2,000 \times 1.05^5 + \left[ 500 – 1,000 \times \left( 1.05^5 – 1 \right) \right] = £2,776$$

Note that the difference between the GMP revaluations and scheme
increases on the GMP can not be used to reduce the pension payable ie
the item in square brackets cannot be negative.


## Full Franking

All of the increases on the pension between retirement and SPA are
franked against revaluation on the GMP.

So, the pension at 65 is calculated as 

$$£2,000 \times 1.05^5 + \left[ 500 - 2,000 \times \left( 1.05^5 – 1 \right) \right] = £2,553$$

Note that the difference between the GMP revaluations and scheme
increases on the whole pension can not be used to reduce the pension
payable i.e. the item in square brackets cannot be negative.


## Maximum

This option differs from Full Franking only if you have an early
retirement decrement in your basis.

For the **early retirements** the calculation assumes there is No
Anti-Franking guarantee. So the pension at 65 is calculated as 

$$£2,000 \times 1.05^5 = £2,553$$

For the **normal retirement** the calculation assumes Full Franking. So
the pension at 65 is calculated as 

$$£2,000 \times 1.05^5 + \left[ 500 – 2,000 \times \left( 1.05^5 – 1 \right) \right] = £2,553$$

Note that the difference between the GMP revaluations and scheme
increases on the whole pension can not be used to reduce the pension
payable i.e. the item in square brackets cannot be negative.


## No Anti Franking Guarantee

No antifranking guarantee is made at SPA.

So, the pension at 65 is calculated as 

$$£2,000 \times 1.05^5 = £2,553$$

## Franking In Deferment

Check this box if you want to allow for franking in deferment. The GMP
benefits will not be added to the other PUPs but will be compared with
the total Excess pension at each age and the greater of the two benefits
valued. This enable the user to value PUPs that pre-date anti-franking
legislation.

The calculations will take account of any pre SPA increases, Barber
Adjustment and the Underpin before comparing the benefits.

The GMP payable on normal or early retirement before SPA may be
different from the GMP at SPA increased in line with statutory
requirements.

## Statutory GMP Increases to NRA>SPA

This field determines the pension increases that are used to increase
the GMP between SPA and NRA for retirements after SPA.

Check the box to increase GMPs by 
1/7%  per week,
then by the assumed statutory GMP increases from SPA to NRA. The
statutory GMP increases are hard-coded in SuperVal and are assumed to be
0% annually for Pre-1988 GMP and 3% annually for Post-1988 GMP.

Leave the box unchecked to increase the GMPs by 1/7%
per week, then by the user specified pension escalation in payment
from SPA to NRA. The pension increases in payment are those specified
for [Pre-1988 GMP](bases+b88gmpinc.md) and [Post-1988 GMP](bases+a88gmpinc.md) 
respectively on the Financial tab.

SuperVal only applies the Late Retirement uplift after the member completes 
seven weeks post state pension age (60 for women and 65 for men) as stated 
in the legislation.

## Public Sector GMPs

Check this box to value public sector style treatment of GMPs. Leave
this box unchecked to value private sector style treatment of GMPs.

This field is only available to some users.

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

## Treat Pre 1988 GMP As Zero

## Treat Post 1988 GMP As Zero

Check these boxes if you want to ignore either the Pre-1988 GMP or the
Post-1988 GMP. (Check both boxes to ignore both.) The GMP will be
assumed to have a zero value.

## Ignore Pre 1988 GMP For Cash Benefit

## Ignore Post 1988 GMP For Cash Benefit

Cash Commutation/Cash on Top is defined on the Ret Cash Tab and can be
either a Percentage or a Multiple of the PUP. Check these boxes if you
wish the Multiple or the Percentage to be based on the PUPs excluding
either the Pre-1988 GMP or the Post-1988 GMP amount. (Check both boxes
to exclude both.) Leave these boxes unchecked to include either the
Pre-1988 GMP or the Post-1988 GMP amount.

Please note that where either the Pre-1988 GMP or the Post-1988 GMP is
included, SuperVal will restrict any pension commuted to ensure that no
GMP is exchanged for cash.

## Ignore Pre 1988 GMP For Death Benefit

## Ignore Post 1988 GMP For Death Benefit

Select how to value both the Pre-1988 GMP and the Post-1988 GMP for
Death Benefits. The options are:

-   Yes
-   No
-   Legislation.

The options are available for the Pre-1988 GMP and Post-1988 GMP
separately.

If `Yes` is selected then no death before retirement benefits will be
payable in respect of either the Pre-1988 GMP or the Post-1988 GMP.

If `No` is selected then SuperVal will value the Pre-1988 GMP or the
Post-1988 GMP multiplied by the [Spouse’s Reversion Death before
Retirement](deferreds_basis+wofrac.md) on death before retirement.

If `Legislation` is selected then the benefits payable on death before
retirement will follow legislation i.e. a 50% spouse’s pension on death
before retirement will be payable in respect of the Pre-1988 GMP for
male members only and a 50% spouse’s pension for all members in respect
of the Post-1988 GMP.

## Pre 1988 Start Date

## Post 1988 Start Date

If you have selected to `Use Barber Start and End Dates` in either the
[Pre-1988 GMP ERF Indicator](#deferreds_basis+bpreind) or the
[Post-1988 GMP ERF Indicator](#deferreds_basis+bpreind) or `Split
According to Service` in the Pre/Post-1988 GMP Underpin Indicator then
SuperVal requires a Start Date and a Finish Date for the Pre-1988 GMP or
the Post-1988 GMP.

The Start Date can either be a fixed date or a data item. To use a fixed
date enter the date here. The date should be in the DD/MM/CCYY format.
To use a data item select from the drop-down list the data item
containing the appropriate data.

SuperVal knows that the Pre-1988 GMP can only have been accrued between
6/4/1978 and 5/4/1988 and that the Post-1988 GMP can only have accrued
between 6/4/1988 and 5/4/1997 and uses this information in the
apportionment.

## Pre 1988 Finish Date

## Post 1988 Finish Date

If you have selected to `Use Barber Start and End Dates` in the either
the [Pre-1988 GMP ERF Indicator](#deferreds_basis+bpreind) or the
[Post-1988 GMP ERF Indicator](#deferreds_basis+bpreind) then SuperVal
requires a Start Date and a Finish Date for the Pre-1988 GMP or the
Post-1988 GMP.

The Finish Date can either be a fixed date or a data item. To use a
fixed date enter the date here. The date should be in the DD/MM/CCYY
format. To use a data item select from the drop-down list the data item
containing the appropriate data.

SuperVal knows that the Pre-1988 GMP can only have been accrued between
6/4/1978 and 5/4/1988 and that the Post-1988 GMP can only have accrued
between 6/4/1988 and 5/4/1997 and uses this information in the
apportionment.

## Pre 1988 ERF Indicator

## Post 1988 ERF Indicator

Select from the drop-down list which set of Early Retirement Reduction
Factors to use for the Pre-1988 GMP or the Post-1988 GMP. The options
are:

-   ERF1
-   ERF2
-   Use Barber Start and End Dates

If `Use Barber Start and End Dates` is selected, the user will be
required to enter these dates on the _Legislation_ tab. In addition, the
user will be required to enter the [Start
Date](#deferreds_basis+prestart) for the GMP benefit and the [Finish
Date](#deferreds_basis+prefinish) for the GMP benefit. For males,
SuperVal will apply ERF2 between Barber Start Date and Barber End Date
and ERF1 for all other periods of service. For females, SuperVal will
apply ERF2 for service prior to the Barber End Date and ERF1 for service
after this date.

## Pre 1988 Dynamism

## Post 1988 Dynamism

This is the rate at which the Pre-1988 GMP or the Post-1988 GMP will
increase between date of retirement and SPA (if later). Select from the
drop-down list which of the previously defined pension increase rates to
use. The options are:

-   Main
-   Special
-   Pension Increase 3
-   Pension Increase 4.

This indicator will also be used to determine which pension any SPA
adjustments for the Pre-1988 GMP or the Post-1988 GMP are made to.

## Pre 1988 Underpin Indicator

## Post 1988 Underpin Indicator

This field is only available if the Benefits Underpinned on the Underpin
Tab has been checked. It will be used to define how the Pre-1988 GMP or
Post-1988 GMP should be treated for Underpin purposes. The options are:

-   Exclude
-   Include
-   Split According To Service

If `Split According To Service` is selected then the user will be
required to enter the Start and Finish Dates for the GMP benefits.
SuperVal will then use these dates to determine the proportion of the
Pre-1988 GMP or Post-1988 GMP that is before or after the Underpin
Commencement Date on the Underpin Tab.

## Pre 1988 GMP Adjustment Factor

## Post 1988 GMP Adjustment Factor

A negative or positive loading can be applied to the Pre-1988 GMP or the
Post-1988 GMP.

Enter the number as a multiplier i.e. `1.1` for a 10% increases or `0.9` for a
10% decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the Pre-1988 GMP or Post-1988 GMP respectively will be
zero.

This field can be used to allow for any contingencies such as children’s
pensions, which are not valued by SuperVal.

## Barber Start Date

This field is used to define the start of the Barber Period after which
males and females must have equal NRA. It will be available when `Use
Barber Start and End dates` is selected for the [ERF
Indicator](deferreds_basis+barbind.md) on the Pups Tab or either the
[Pre-1988 ERF Indicator](#deferreds_basis+bpreind) or the [Post-1988
ERF Indicator](#deferreds_basis+bpreind) on the Legislation Tab.

For most schemes the Barber Start Date will be 17/05/1990. Enter the
Barber Start Date in DD/MM/YYYY format.

Where an early retirement decrement applies, Early Retirement Pension
Reduction Factors will need to be specified separately for males and
females for the periods

-   prior to Barber Date
-   inside the Barber Window i.e. 17/5/1990 to the date of equalisation
    and
-   after the date of equalisation i.e. Barber End Date.

For males, SuperVal will apply ERF2 between Barber Start Date and Barber
End Date and ERF1 for all other periods of service. For females,
SuperVal will apply ERF2 for service prior to the Barber End Date and
ERF1 for service after this date.

## Barber End Date

This field is used to define the end of the Barber Period after which
males and females must have equal NRA. It will be available when `Use
Barber Start and End dates` is selected for the [ERF
Indicator](deferreds_basis+barbind.md) on the Pups Tab or either the
[Pre-1988 ERF Indicator](#deferreds_basis+bpreind) or the [Post-1988
ERF Indicator](#deferreds_basis+mpreind) on the Legislation Tab.

Enter the Barber End Date in DD/MM/YYYY format.

Where an early retirement decrement applies, Early Retirement Pension
Reduction Factors will need to be specified separately for males and
females for the periods

-   prior to Barber Date
-   inside the Barber Window i.e. 17/5/1990 to the date of equalisation
    and
-   after the date of equalisation i.e. Barber End Date.

For males, SuperVal will apply ERF2 between Barber Start Date and Barber
End Date and ERF1 for all other periods of service. For females,
SuperVal will apply ERF2 for service prior to the Barber End Date and
ERF1 for service after this date.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

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