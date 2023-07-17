# Edit UKPUP



## PUP Description

Up to 20 separate Benefits can be specified.

Enter a description for the pension benefit being valued eg Post-97
pension.

This description will appear on the results output.

Note: The benefits on the Ind PUPs Tab can only be edited if the
[Independent PUPs](deferreds_basis+indpups.md) box on the Main Tab has
been checked.

## PUP Amount

Select from the drop-down list the data item to be valued. The data item
should contain the excess over the GMP.

## Revaluation Rate Override

The user has the option to enter an override for the [Excess
Revaluation](deferreds_basis+revn.md) Rate entered on the Financial
tab.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

If you do not wish to use this option then leave blank.

## Spouses DAR Override

The user has the option to enter an override for the [Spouse’s Death
after Retirement Percentage](deferreds_basis+warfrac.md) entered on the
Ret Pension Tab.

Either enter the fixed percentage override or select from the drop-down
list the data item that contains the appropriate data for this PUP. If
the override is fixed for all members, enter as a percentage i.e. for 50%
enter `50` rather than `0.5`. (Note for Ind Pups only a fixed percentage can
be used.)

If you do not wish to use this option then leave blank.

## Override % for DBR Pension

The user has the option to enter an override for the [Spouse’s Death
before Retirement Percentage](deferreds_basis+wofrac.md) entered on the
Death Tab.

Either enter the fixed percentage override or select from the drop-down
list the data item that contains the appropriate data for this Pup. If
the override is fixed for all members, enter as a percentage i.e. for 50%
enter `50` rather than `0.5`.

If you do not wish to use this option then leave blank.

## Complete Years Only Override

The user has the option to enter an override for the [Count Complete
Years](deferreds_basis+revyrs.md) entered on the Financial Tab.

Exits before NRA such as early retirement and death in deferment are
assumed to occur half-way through the year i.e. 0.5, 1.5, 2.5 years after
the valuation date. By selecting `Yes` these benefits will receive
revaluations for the number of complete years only i.e. 0, 1, 2. By
selecting `No` these benefits will receive an additional half-year of
revaluations i.e. 0.5, 1.5, 2.5.

If you do not wish to use this option then leave blank.

## NRA Exits Rounding Override

The user has the option to enter an override for the [NRA Exits
Rounding](deferreds_basis+nrarnd.md) entered on the Financial Tab.

Select from the drop-down list how the override rounding for exits at
NRA should be calculated. The revaluation of the PUP to Normal
Retirement Age will be based on the exact duration between Valuation
Date and Normal Retirement Date, rounded according to the parameter
entered. The options are:

-   Exact Days
-   Months Rounded Down
-   Nearest Months
-   Months Rounded Up
-   Years Rounded Down
-   Nearest Years
-   Years Rounded Up
-   Complete Tax Years

The discounting of the benefit will be based on years nearest.

If you do not wish to use this option then leave blank.

## Start Date

If either the [ERF Indicator](#deferreds_basis+barbind) (or the GMP
ERF Indicators) are set to `Use Barber Start and End Dates` or the
[Include in Underpin](#deferreds_basis+undind) is set to `Split
According to Service` then SuperVal requires a Start Date and a Finish
Date for each of the PUPs.

The Start Date can either be fixed for all members or variable. Enter a
fixed date in the form DD/MM/YYYY. To enter a variable date, select from
the drop-down list the appropriate data item.

## Finish Date

If the [ERF Indicator](#deferreds_basis+barbind) (or the GMP ERF
Indicators) are set to `Use Barber Start and End Dates` or the [Include
in Underpin](#deferreds_basis+undind) is set to `Split According to
Service` then SuperVal requires a Start Date and a Finish Date for each
of the PUPs.  
The Finish Date can either be fixed for all members or variable. Enter a
fixed date in the form DD/MM/YYYY. To enter a variable date, select from
the drop-down list the appropriate data item.

## PUP Adjustment Factor

A negative or positive loading can be applied to the PUP.

Enter the number as a multiplier i.e. `1.1` for a 10% increase or `0.9` for a
10% decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the PUP will be zero.

This field can be used to allow for any contingencies, such as
children’s pensions, which are not valued by SuperVal.

## Ignore for Cash

The cash calculations are defined on the Ret Cash Tab.

Check this box if you do not want to include this PUP in the cash
calculations. Leave the box unchecked if you do want to include this PUP
in the cash calculations.

## Ignore for DBR

Check the box if you do not want to include this PUP in the Death Before
Retirement benefits. Leave the box unchecked if you do want to include
this PUP in the Death Before Retirement benefits.

## ERF Indicator

Select from the drop-down list which set of Early Retirement Reduction
Factors to use. The options are

-   ERF1
-   ERF2
-   Use Barber Start and End Dates.

ERF1 and ERF2 are specified on the Ret Pension Tab.

If `Use Barber Start and End Dates` is selected, the user will be
required to enter these dates on the Legislation Tab. For males,
SuperVal will apply ERF2 between Barber Start Date and Barber End Date
and ERF1 for all other periods of service. For females, SuperVal will
apply ERF2 for service prior to the Barber End Date and ERF1 for service
after this date. In addition, the user will be required to specify the
[Start Date](#deferreds_basis+indstart) and [Finish
Date](#deferreds_basis+indfinish) for the PUP.

## Pension Increases in Payment

Once in payment, the pension from this Slice or PUP, can be set to
increase at one of four different increase rates. Select from the
drop-down list the appropriate rate. The options are:

-   Main Pension
-   Special Pension
-   Pension Increase 3
-   Pension Increase 4

## Include In Underpin

Select from the drop-down list how the PUP should be treated in the
Underpin comparison. The options are:

-   Exclude
-   Include
-   Split According to Service

If `Split According to Service` is selected then enter the [Start
Date](#deferreds_basis+indstart) and [Finish
Date](#deferreds_basis+indfinish) above and the [Underpin
Commencement Date](bases+mpudate.md) on the Underpin Tab.

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

## Next PUP

Move on to the next PUP. Select "ok" to save any changes to the current PUP.

## Previous PUP

Move back to the previous PUP. Select "ok" to save any changes to the current PUP.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

## OK

When you have finished entering the relevant information, click the _OK_
button to move to the next screen.

SuperVal will check that all of the required entries on the page have
been made. If additional fields require data SuperVal will show briefly
in red which is the first of these fields found on the page.

## Cancel

Clicking on the _Cancel_ button allows you to return to the previous
screen without saving any of your changes.