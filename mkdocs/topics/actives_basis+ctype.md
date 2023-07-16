# Retirement Cash Benefit Basis

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
