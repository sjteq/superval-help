# Deferreds Basis: NSPUPs



## PUP Amount

Select from the drop-down list the data item to be valued as a
non-standard Death before Retirement pension.

## % of PUP Amount

This field is used to determine the percentage of the data item that is
paid to a spouse as a death before retirement pension. Enter the
percentage here, for 50% enter `50`.

Note where 100% is entered, the data item will be valued as death before
retirement pension only i.e. a member’s single life pension will _not_ be
valued in addition.

## Revaluation Rate Override

The user has the option to enter an override for the [Revaluation
Rate](deferreds_basis+revn.md) entered on the Financial Tab. This will
be used to increase the death before retirement pension prior to NRA.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Complete Years Only Override

The user has the option to enter an override for the [Count Complete
Years](deferreds_basis+revyrs.md) entered on the Financial Tab.

Exits before NRA such as early retirement and death in deferment are
assumed to occur half way through the year i.e. 0.5, 1.5, 2.5 years after
the valuation date. By selecting `Yes` these benefits will receive
revaluations for the number of complete years only i.e. 0, 1, 2. By
selecting `No` these benefits will receive an additional half-year of
revaluations i.e. 0.5, 1.5, 2.5.

If you do not wish to use this option then leave blank.

## Pension Increases in Payment

Once in payment, the Non Standard Death before Retirement Pension, can
be set to increase at one of four different increase rates. Select from
the drop-down list the appropriate rate. The options are:

-   Main Pension
-   Special Pension
-   Pension Increase 3
-   Pension Increase 4

## Adjustment Factor

A negative or positive loading adjustment can be applied to the Death
Before Retirement Pension.

Enter the number as a multiplier i.e. for `1.1` for a 10% increase or `0.9`
for a 10% decrease. If no adjustment is required enter `1`. If `0` is
entered the liability for the Death Before Retirement Pension will be
zero.

This field can be used to allow for any contingencies such as children’s
pensions, which are not valued by SuperVal.

## Treat as Post 1997 for CAP

Check this box if this Non Standard Death Before Retirement Pension
should be treated as a Post-1997 pension when running a Non PPF (Capped)
Valuation. Leave unchecked if this benefit should be treated as Pre-1997
pension.

## PUP Amount

Select from the drop-down list the data item to be valued as a
non-standard Death after Retirement pension.

## % of PUP Amount

This field is used to determine the percentage of the data item that is
paid to a spouse as a death after retirement pension. Enter the
percentage here, for 50% enter `50`.

Note where 100% is entered, the data item will be valued as death after
retirement pension only i.e. a members single life pension will _not_ be
valued in addition.

## Revaluation Rate Override

The user has the option to enter an override for the [Revaluation
Rate](deferreds_basis+revn.md) entered on the Financial Tab. This will
be used to increase the death after retirement pension prior to NRA.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Complete Years Only Override

The user has the option to enter an override for the [Count Complete
Years](deferreds_basis+revyrs.md) entered on the Financial Tab.

Exits before NRA such as early retirement and death in deferment are
assumed to occur half way through the year i.e. 0.5, 1.5, 2.5 years after
the valuation date. By selecting `Yes` these benefits will receive
revaluations for the number of complete years only i.e. 0, 1, 2. By
selecting `No` these benefits will receive an additional half-year of
revaluations i.e. 0.5, 1.5, 2.5.

If you do not wish to use this option then leave blank.

## Exit Rounding Override

The user has the option to enter an override for the [NRA Exits
Rounding](deferreds_basis+nrarnd.md) entered on the Financial Tab.

Select from the drop-down list how the rounding for exits at NRA
Override should be calculated. The revaluation of the PUP to Normal
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

## ERF Indicator

Select from the drop-down list which set of Early Retirement Reduction
Factors to apply to the Death after Retirement benefits. The options
are:

-   None
-   ERF1
-   ERF2

ERF1 and ERF2 are specified on the Ret Pension Tab.

Note, the option to `Use Barber Start and End Dates` to determine the
Early-Retirement Factors used is not available for Death after
Retirement pensions specified on this Tab. If this is required, the user
should load separate data items and value with different
Early-Retirement Factors.

## Pension Increases in Payment

Once in payment, the Non Standard Death after Retirement Pension, can be
set to increase at one of four different increase rates. Select from the
drop-down list the appropriate rate. The options are:

-   Main Pension
-   Special Pension
-   Pension Increase 3
-   Pension Increase 4

## Adjustment Factor

A negative or positive loading can be applied to the NSPUP.

Enter the number as a multiplier i.e. `1.1` for a 10% increase or `0.9` for a
10% decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the PUP will be zero.

This field can be used to allow for any contingencies, such as
children’s pensions, which are not valued by SuperVal.

## Treat as Post 1997 for CAP

Check this box if this Non Standard Death After Retirement Pension
should be treated as a Post-1997 pension when running a Non PPF (Capped)
Valuation. Leave unchecked if this benefit should be treated as Pre-1997
pension.

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