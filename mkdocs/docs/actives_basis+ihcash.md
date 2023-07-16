# Actives Basis: IHCash



## Ill-Health Cash Parameter Set

Cash Parameter Set is a Scheme Global parameter which groups the
Retirement Cash Commutation variables. This can be created by using
either the `Create Globals` function or using the _Add/Edit Retirement
Cash_ button. Once created, these parameters can be edited without going
back into the Basis similar to other global parameter sets.

## Benefit Basis

A lump sum cash benefit can be paid at retirement either through
commutation (ie exchange of pension for cash) or in addition to the
pension benefits. Select from the drop-down list the basis of
calculating any cash benefit provided. The options are:

-   Neutral or Nil
-   25% of Pension
-   IR Maximum
-   2.25 &times; Pension
-   Accrual &times; Salary for each year
-   3 &times; Pension
-   Multiple of Pension
-   % of Pension

When using the `IR Maximum option` the user will need to set up the [IR
Maximum Parameters Rules](actives_basis+irmaxind.md).

When using the `Accrual × Salary for each year`, the user will be
required to enter the salary, service and accrual rate on which this is
based. Note that if using this option, ERF factors will not be applied
to the cash on top lump sum. (If you do want ERFs to be applied to cash
on top, you could use the Multiple of pension option instead.)

When using the `Multiple of Pension`, the Multiple can either be fixed
for all members or be a member specific amount. To use a fixed Multiple,
enter the value. To use a Member Specific Multiple, select from the
drop-down list the data item containing the appropriate data.

When using the `% of Pension`, the Percentage can either be fixed for
all members or be a member specific amount. To use a fixed Percentage,
enter the value. To use a Member Specific Percentage, select from the
drop-down list the data item containing the appropriate data.

When using `25% of Pension` or `% of Pension`, the amount of cash lump
sum will be determined by the Commutation Tables specified.

For all of these options you can select whether to [Ignore GMP in
Split.](#actives_basis+cgmp) The Commutation will be restricted to
avoid commuting the GMP, however there is no allowance for
post-retirement increases in calculating this restriction. In addition,
you will be required to specify the [Commutation
Priority](#bases+cashp) and the Commutation Tables to use.

Finally, where benefits for both Cash On Top of pension and Cash
Commutation are specified the Cash Commutation is calculated first. If
the Cash On Top formula relates to the amount of pension this will be
based on the pension prior to commutation.

## On Top or Commuted

Select from the drop-down list which of the cash option to use. The
options are:

-   On Top
-   Commuted

If `Commuted` is selected, the amount of pension commuted will be
restricted to the excess over GMP and then the user will be able to
select the [Commutation Priority](#bases+cashp).

## Accrual Rate

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Enter the percentage of salary to be
used in the calculation of cash for each year of service i.e. for 3/80ths
use `0.0375`.

When using this option, Early-Retirement Factors will not be applied to
the cash-on-top benefit.

## Salary

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Select from the drop-down list the
salary to be used in the calculation of cash for each year of service.

When using this option, Early-Retirement Factors will not be applied to
the cash-on-top benefit.

## Service

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Select from the drop-down list the
service to be used in the calculation of cash for each year of service.
The options are:

-   Scheme Membership
-   Company Service

Note that total service from either Date Joined Scheme or Date Joined
Company will be used in these calculations.

When using this option, Early-Retirement Factors will not be applied to
the cash-on-top benefit.

## Cash Multiple

This field is only required if the Cash Calculations are based on a
`Multiple of Pension`. The Multiple can either be fixed for all members
or member specific.

To use a fixed multiple, enter the multiple here. (Using a multiple of 3
is the same as selecting `3 &times; pension`.)

To value a member specific multiple, select from the drop-down list the
data item containing the appropriate data.

## Cash Percentage

This field is only required if the Cash Calculations are based on a `%
of Pension`. The Percentage can either be fixed for all members or a
member specific percentage.

To value a fixed percentage for all members, enter the percentage here
ie for 25% enter `0.25`.

To value a member-specific percentage, select from the drop-down list
the data item containing the appropriate data.

## Include Prospective Service

This field allows the user to specify whether the commuted cash or cash
on top calculations will include the ill health prospective service when
the Ill Health [Benefit Basis](actives_basis+illind.md) is either a
Prospective Pension or a Prospective Table.

Check the box to include prospective service. Leave the box unchecked to
exclude prospective service.

## Separate A-Day Cash Factors for each Pension Increase

This field indicates if separate A Day cash factors are to be calculated
for each pension increase or whether a single factor applies to the
entire pension.

 

If a User opts for the average factor approach which means the field is
left unchecked, then the User needs to select whether the average factor
will be applied Pro Rata or Priority.

## Treat Independent Slice Cash as Cash on Top

Users sometimes value Cash on Top in the Ind Slices and Ind PUPs giving
data items the same payment start and end age. If the intention is to
include this Cash on Top amount in the A Day max calculation, then this
box should be checked.

If this box is unchecked the system will still value cash amounts in the
Ind Slices and Ind PUPs but the A Day maximum will not be reduced to
allow for this Cash on Top (if the basis has `Percentage of A Day Cash`
commutation specified).

## Commutation Priority

This field is used to determine the order in which pension will be
commuted for cash. Select from the drop-down list which of the options
to use. The options are:

-   After Split (actives only)
-   Before Split (actives only)
-   Priority
-   Pro Rata

If `After Split` or `Before Split` is used then the pension is commuted
by reference to the `Latest Finish Date` specified on the [Offset
Slice](actives_basis+sliceup.md).

Typically an active member will have a service timeline as shown in the
following diagram:

![](img/bm6.gif)

If `After Split` is selected then the pension accrued after the End of
the Offset Slice would be commuted first. Within each period pension may
increase at different rates and are commuted in the following order:

-   Special
-   Main
-   Pension Increase 3
-   Pension Increase 4

If `Before Split` is selected then the pension accrued before End of the
Offset Slice would be commuted first. Within each period pension may
increase at different rates and are commuted in the following order:

-   Special
-   Main
-   Pension Increase 3
-   Pension Increase 4

If `Priority` is selected then the cash is commuted according to the
pension increase rate applied on the Slices or PUP Tab. Pensions are
commuted in the following order:

-   Special
-   Main
-   Pension Increase 3
-   Pension Increase 4

If `Pro Rata` is selected, then pension is commuted in proportion to the
pension amounts, irrespective of the pension increase rate.

## Ignore GMP in Split

This field enables the split between Pre-97 and Post-97 benefit to be
done in the correct proportions. Check this box if SuperVal should
ignore the GMP when calculating cash proportions. Please note that if
this option is chosen then the GMP pension maybe commuted. (This depends
on the options chosen and the size of the GMP.) However, SuperVal will
still pay the whole of the GMP at SPA. This may overstate the liability.

## Male Reduction Factors

## Female Reduction Factors

## Ill Health Cash on Top Reduction Factors

This field allows the user to specify a set of early retirement
reduction factors that apply to Ill Health Cash-on-Top benefit.
Typically, where this is unreduced the factors would be 1 at all ages.
Double click to select from the list of available tables.

If the field is left blank then SuperVal will assume 1 at all ages.

If the Ill Health Cash-on-Top benefit is defined as Accrual &times; Salary for
each year of service then no Early-Retirement Factors can be applied.

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

## Linearly Interpolate Reduction Factors for mid-point Exit values

## Linearly Interpolate Male Commutation Tables for mid-point Exit values

## Linearly Interpolate Female Commutation Tables for mid-point Exit values

When checked, the system will linearly interpolate factors for mid year
exits such as early retirements and deaths. For Normal Retirements, the
system will apply no interpolation. If unchecked, the system will use
the factor specified at the age nearest rounded down for mid year exits
as previous versions have done.

## Male Ill-Health Commutation Tables Parameter Set

## Female Ill-Health Commutation Tables Parameter Set

Commutation Tables Parameter Set is a Scheme Global parameter which
groups the Male or Female Commutation table variables. This can be
created by using either the `Create Globals` function or using the
_Add/Edit Commutation Table_ button.

Once created, these parameters can be edited without going back into the
Basis similar to other global parameter sets.

## Calculate Male Commutation Factors based on Valuation Basis

## Calculate Female Commutation Factors based on Valuation Basis

SuperVal will calculate commutation factors applicable to each
individual member using the valuation basis and the all relevant Basis
Parameters (Guarantee Period, Post Retirement Mortality, Post Retirement
Interest rate and Pension Increases).

## Male % of Valuation Basis Factor

## Female % of Valuation Basis Factor

Users
can define the % of Valuation Basis Factor they want to apply to the
Scheme. To have this field visible the above field `Calculate
Male/Female Commutation Factors based on Valuation Basis` needs to be
ticked. The Valuation Factors produced by SuperVal can be seen in
individual VARPRINTs.

## Male Main

## Male Special

## Male PenInc3

## Male PenInc4

## Female Main

## Female Special

## Female PenInc3

## Female PenInc4

Double click to select the rate table containing the Commutation Factors
ie the amount of cash received for each pound per annum of pension
commuted.

For example, a factor of 9 at age 65 means that for every pound
surrendered in pension at age 65 the member would receive £9 in cash.

Separate tables can be specified for males and females and for each of
the different pension increase rates (Main, Special, Pension Increase 3
and Pension Increase 4) being used.

NB: Even if cash is payable on top of pension benefits, cash commutation
factors are still required for application of IR Maximum rules.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Adjust Male Commutation Tables by the change in member's expectation of life

## Adjust Female Commutation Tables by the change in member's expectation of life

Future mortality-improvement assumptions underlying the Technical Provisions can be applied to the tabulated commutation factors in force at the valuation date, to calculate revised commutation factors at the date of exit.

## Add/Edit Retirement Cash

Add or Edit any Retirement Cash parameter sets

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