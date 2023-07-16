# Deferreds Basis: IndPUPs



## Independent PUP Description

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

## Male Start Age

## Female Start Age

This is the age at which the Independent Pup being described will come
into payment. This can either be a fixed date for all members or an age
specific for each member.

To use a fixed age for all members, enter the age here.

To use a member’s specific age, select from the drop-down list the data
item containing the member specific age.

Note, to value a cash benefit the Payment Start Age should be set equal
to the Payment End Age.

## Male End Age

## Female End Age

This is the age at which the Independent Pup being described will stop
being paid.

This can either be a fixed date for all members or an age specific for
each member. To use a fixed age for all members, enter the age here. To
use a member’s specific age, select from the drop-down list the data
item containing the member specific age.

Note, to value a cash benefit the Payment Start Age should be set equal
to the Payment End Age.

## PUP Adjustment Factor

A negative or positive loading can be applied to the PUP.

Enter the number as a multiplier i.e. `1.1` for a 10% increase or `0.9` for a
10% decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the PUP will be zero.

This field can be used to allow for any contingencies, such as
children’s pensions, which are not valued by SuperVal.

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

## Add PUP

Clicking on the _Add PUP_ Button allows you to add another PUP definition.
Select whether to use the default pension definition or one of the
existing PUP definitions as the starting point.

## Insert PUP

Clicking on the _Insert PUP_ button allows you to insert another PUP
definition.

Select from the list of PUPs the PUP definition you want to insert the
new PUP before.

## Edit PUP

Pressing the _Edit PUP_ button allows you to edit a PUP definition.

You must select the PUP definition to be edited, unless a PUP definition
is currently highlighted, in which case this PUP definition will be
edited.

## Delete PUP

Clicking the _Delete PUP_ button allows you to, after confirmation, delete
a PUP.

You must select the PUP to be deleted, unless a PUP is currently
highlighted, in which case this PUP will be deleted.

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