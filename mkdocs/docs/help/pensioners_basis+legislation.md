# Pensioners Basis: Legislation



## Fixed Revaluation Rate to SPA

Check this box if the GMP Revaluation Rate to SPA is Fixed.

The revaluation rate will be determined by SuperVal for each member
based on the data contained in the standard data item `LD` - Leaving
Date.

If unchecked, the user will be required to enter the rate of revaluation
to use in GMP [Revaluation Rate to SPA](#pensioners_basis+gmprev1).

## Revaluation Rate to SPA

This is the rate at which the GMP will be revalued to SPA when Fixed
Rate Revaluations do not apply.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Revaluation Rate  when BAGE<SPA

This field only applies to normal/early retirement pensions before SPA.
It is not used for death in deferment benefits. If GMP retirement
benefits payable before SPA are determined using a different rate of
revaluation to that used to SPA then that different rate should be
entered here.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

If this field is left blank, SuperVal will use the [Revaluation Rate to
SPA](#pensioners_basis+gmprev1).

## Reduce Pensions at SPA

Check this box if the pensions defined on the Pensions Tab will be
reduced at SPA (or earlier death) when the GMP comes into payment. If
this option is selected the [Use Approximate GMP
Ratio](#pensioners_basis+gmpsplit) check box becomes available. This
can be used to approximate the GMP offset from each of the pensions if
this data is unavailable.

If the GMP data underlying each of the pensions in available then the
user will be required to enter this in the [Pre/Post-1988 Included at
Retirement](pensioners_basis+preret.md) and [Pre/Post Included at
Valuation Date](pensioners_basis+prevd.md).

Leave the box unchecked if there are no GMPs or if the GMPs are to be
paid in addition to the pensions specified on the Pensions Tab.

## Use Approximate GMP Ratio

When the [Reduce Pensions at SPA](#pensioners_basis+puprdn) on the
Legislation Tab is checked and the underlying GMP for each of the
pensions on the Pensions Tab is not available, SuperVal can use an
approximate allocation of the total GMPs to those pensions where
[Include in Adjustment at SPA/Death](pensioners_basis+gmpadj.md) on the
Pension Tab is selected.

To use this functionality, check this box. The user will then be
required to enter Pseudo GMPs at both retirement and the valuation date
below.

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

## Male PPF NRA

## Female PPF NRA

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

## Pre 1988 Total Pseudo Amounts at Retirement

This field is only required if [Use Approximate GMP
Ratio](#pensioners_basis+gmpsplit) is checked.

Select from the drop-down list the data item containing the total
Pre-1988 GMP underlying the pensions at retirement for members who have
not yet reached SPA.

## Pre 1988 Total Pseudo Amounts at Valuation Date

This field is only required if [Use Approximate GMP
Ratio](#pensioners_basis+gmpsplit) is checked.

Select from the drop-down list the data item containing the total
Pre-1988 GMP underlying the pension at Valuation Date for members who
have not yet reached SPA. This will enable the correct adjustment
(subject to Franking Code) to be made at SPA.

This GMP can be different from the standard GMP data items (GMP0 and
GMPE0).

For example, a member who retires from deferred status before SPA where
the GMP revaluations from date of leaving are not payable until SPA.

## Pre 1988 GMP Adjustment Factor

A negative or positive loading can be applied to the Pre-1988 GMP.

The entered adjustment is applied to the standard data item. Enter the
number as a multiplier i.e. `1.1` for a 10% increase or `0.9` for a 10%
decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the Pre-1988 GMP will be zero.

This field can be used to allow for any contingencies, such as
children’s pensions, which are not valued by SuperVal.

## Post 1988 Total Pseudo Amounts at Retirement

This field is only required if [Use Approximate GMP
Ratio](#pensioners_basis+gmpsplit) is checked.

Select from the drop-down list the data item containing the total
Post-1988 GMP underlying the pension at retirement for members who have
not yet reached SPA.

## Post 1988 Total Pseudo Amounts at Valuation Date

This field is only required if [Use Approximate GMP
Ratio](#pensioners_basis+gmpsplit) is checked.

Select from the drop-down list the data item containing the total
Post-1988 GMP underlying the pensions at Valuation Date for members who
have not yet reached SPA. This will enable the correct adjustment
(subject to Franking Code) to be made at SPA.

This GMP can be different from the standard GMP data items (GMP0 and
GMPE0).

For example, a member who retires from deferred status before SPA where
the GMP revaluations from date of leaving are not payable until SPA.

## Post 1988 GMP Adjustment Factor

A negative or positive loading can be applied to the Post-1988 GMP.

The entered adjustment is applied to the standard data item. Enter the
number as a multiplier i.e. `1.1` for a 10% increase or `0.9` for a 10%
decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the Post-1988 GMP will be zero.

This field can be used to allow for any contingencies, such as
children’s pensions, which are not valued by SuperVal.

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