# Retirement Cash



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
Split.](actives_basis+cgmp.md) The Commutation will be restricted to
avoid commuting the GMP, however there is no allowance for
post-retirement increases in calculating this restriction. In addition,
you will be required to specify the [Commutation
Priority](bases+cashp.md) and the Commutation Tables to use.

Finally, where benefits for both Cash On Top of pension and Cash
Commutation are specified the Cash Commutation is calculated first. If
the Cash On Top formula relates to the amount of pension this will be
based on the pension prior to commutation.

## Accrual Rate

This field is only required if the Cash Calculations are based on
`Accrual × Salary for each year`. Enter the percentage of salary to be
used in the calculation of cash for each year of service i.e. for 3/80ths
use `0.0375`.

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

## Separate A-Day Cash Factors for each Pension Increase

This field indicates if separate A Day cash factors are to be calculated
for each pension increase or whether a single factor applies to the
entire pension.

 

If a User opts for the average factor approach which means the field is
left unchecked, then the User needs to select whether the average factor
will be applied Pro Rata or Priority.

## Treat Independent Slice/PUP Cash as Cash on Top

Users sometimes value Cash on Top in the Ind Slices and Ind PUPs giving
data items the same payment start and end age. If the intention is to
include this Cash on Top amount in the A Day max calculation, then this
box should be checked.

If this box is unchecked the system will still value cash amounts in the
Ind Slices and Ind PUPs but the A Day maximum will not be reduced to
allow for this Cash on Top (if the basis has `Percentage of A Day Cash`
commutation specified).

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