# Actives Basis: Legislation



## Revaluation Type to SPA

Select from the drop-down list how to revalue the GMPs for members who
leave active service before SPA. The options are:

-   None
-   Fixed
-   Limited
-   S148

If `Fixed` Rate revaluations are selected SuperVal will use the
following rates to revalue the pension (based on member’s year of exit):

Leaving Service Date  | Revaluation Rate
----------------------|-----------------
Post-06/04/2012       | 4.75%
06/04/2007–05/04/2012 | 4.00%
06/04/2002–05/04/2007 | 4.50%
06/04/1997–05/04/2002 | 6.25%
06/04/1993–05/04/1997 | 7.00%
06/04/1988–05/04/1993 | 7.50%
Pre-06/04/1988        | 8.50%

If `Limited` is selected, then please note LRPs will not be calculated.
This option is intended to give the user an indication of the difference
between Fixed and Limited revaluations.

If `S148` increases are selected then enter the appropriate rate of
increase in the field [Section 148 orders](#actives_basis+s148).

## Section 148 Orders

This is the rate at which GMPs for members in active service and for
leavers with revaluations in line with S148 orders will be increased.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Revalue to NRA<SPA

Check this box if NRA is less than SPA and the GMP is revalued at a
different rate to NRA. If NRA is equal to SPA then leave this field
unchecked and the statutory revaluation will be correctly applied.

If checked, SuperVal will apply the [Revaluation Rate to NRA&lt;
SPA](#actives_basis+gmprevalrat) to the GMP up to NRA. Then at SPA it
will make an addition for all the statutory revaluations on the GMP not
yet in payment (subject to the [Franking Code](#bases+offcod) ).

## Revaluation Rate to NRA<SPA

This is the rate at which GMP benefits will be revalued to NRA if the
[Revalue to NRA&lt;SPA](#actives_basis+gmpdefind) box has been
checked. At SPA, SuperVal will revalue the GMP using the [Revaluation
Type to SPA](#actives_basis+grev) selected. Any shortfall in
revaluations (when compared to the GMP at NRA) will be added to the PUP
at SPA. The addition at SPA would be subject to the [Franking
Code](#bases+offcod).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this Tab.

An example to illustrate this is set out below:

Suppose you have a male member who is currently 30 who will retire at
age 60. All of his pension is revalued in deferment at 3.5% pa. The user
has checked the Revalue to NRA&lt;SPA box and has selected a Global
Financial Parameter with a value of 3.5% for this field. The GMP
revaluation type is fixed. The pension accrued in the 2nd year is £1,000
of which £500 is GMP. Once in payment, the pension will increase at 4%
per annum.

The deferred PUP payable at age 60, after leaving in the second year,
will be calculated as 

$$ £1,000 \times 1.035^{28} = £2,620 $$

(Note that GMP is revalued using complete years in the same way
as the excess over GMP.)

The addition at SPA for GMP revaluations not yet in payment, assuming no
franking, is calculated as 

$$£500 \times 1.045^{32} - £500 \times 1.035^{28} = £735$$

(Note that complete tax
years are used for the revaluation of the GMP to SPA.)

The deferred PUP at SPA will be calculated as 

$$£2,620 \times 1.04^5 + £735 = £3,923$$

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

## Offset Slices

## Offset Slice Number

This field is used to identify the date at which the GMP accrual
ceased.  Enter the Slice Number on which the [Service Finish
Date](actives_basis+fndate.md) should be used as the date at which GMP
accrual has ceased.  All of the benefits arising from the Slice entered
and higher Slice Numbers will be assumed to have an underlying GMP
benefit.  (Including those Slices where only added years and pension
data item benefits are specified.)

For example, if there are four Slices specified as follows:

slice | specification
------|--------------
1     | Future Service, i.e. `VDATE` to `LDATE`
2     | Service from 6/4/1997 (or `DJF` if later) to `VDATE`
3     | Service from a benefit/category change date (or `DJF` if later) to 6/4/1997
4     | Service from `DJF` to the benefit/category change date

The Offset Slice Number entered is 3, meaning that the benefits under
Slices 3 and 4 will have GMP underlying them.  The benefits under Slices
1 and 2 will not have GMP benefits.

Where the Scheme is Contracted-In and/or GMP benefits are payable on top
of the benefits entered on the Slices, enter a value of `17`.   

Please note that this field is used in a Non PPF Capped Valuation Run to
determine which parts of the pension receive pension increases.  Pension
arising from Slices before the `Offset Slice` number and higher will be
deemed to have no pension increases for PPF Valuation purposes. Pension
arising from a Slice number lower than the `Offset Slice` will be deemed
to be increasing pension in payment for PPF Valuation purposes.

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

## Treat GMPs As Zero

Check this box to ignore all GMP benefits. Leave unchecked if you want
to value GMP benefits.

## Public Sector GMPs

Check this box to value public sector style treatment of GMPs. Leave
this box unchecked to value private sector style treatment of GMPs.

This field is only available to some users.

## Rules

Select from the drop-down list which of the pre-A-Day Inland Revenue
Limits to apply. The limits will be applied to the retirement pensions
calculated by SuperVal in the Benefit Slices for the corresponding
periods of service. The options are:

-   Ignore
-   Pre-1987 Rules
-   Pre-1987 or Post-1989, depending on DJF
-   Post-1987 or Post-1989, depending on DJF
-   Post-1989 Rules
-   Pre-1987, Post-1987 or Post-1989, depending on DJF

The IR maximum pension will be calculated according to the option
chosen. The Date Joined Company (DJS) is used in the calculation of the
maximum.

The Post-A-Day Tax Simplification Rules are not calculated by
SuperVal. However, there is an option to use either a percentage or
multiple data item for the cash benefit percentage which could be
manipulated to approximate this benefit.

## Cap Increase Rate

Inland Revenue Limits for joiners Post-31/05/1989 are calculated using
the Earnings Cap. This is the rate at which the Earnings Cap will
increase to date of exit.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this Tab.

The Earnings Cap, to which this rate is applied, is taken from the
Factor File. The Factor that contains the Earnings Cap is called Max.
Please note that the calculations determine the total benefit amount for
Post-1989 joiners using the Earnings Cap figure but do not restrict the
actual salary used in the calculations to the Earnings Cap. In order to
limit the salary used to the Earnings Cap set a Salary Maximum on the
Salaries Tab.

## Salary

Select from the drop-down list which of the salaries defined on the
Salaries Tab should be used to calculate the Inland Revenue maximum
pension.

## Application

Select from the drop-down list how to apply the Inland Revenue Maximum
Rules to the retirement and cash benefits. The options are:

-   Limit Future First
-   Proportionate

Under `Limit Future First` the future service benefit will be restricted
by the Inland Revenue Limit Maximum first.

Under `Proportionate` any Inland Revenue Limit will apply
proportionately to past and future service benefits.

Consider the following example:

 &nbsp;                | Prior to application | Limit Future First | Proportionate
-----------------------|---------------------:|-------------------:|-------------:
Total Service Pension  | £12,000
Future Service Pension | £7,000               | £5,000             | £5,833
Past Service Pension   | £5,000               | £5,000             | £4,167
IR Maximum Pension     | £10,000              | £10,000            | £10,000

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