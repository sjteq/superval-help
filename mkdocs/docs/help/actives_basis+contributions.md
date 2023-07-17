# Actives Basis: Contributions



## Member Contributions Definition

Select from the drop-down list the Global Contribution Definition that
contains the member’s contribution parameters.

The Global Contribution Definition will contain the Method to calculate
contributions and any additional parameters required to define the
contributions.

To add a new Global Contribution Definition use the _Edit Contribution
Definition_ button at the bottom of this Tab.

For more information please see the Infocus Document relating to Setting
Up Contribution Definitions.

## Member Conts Salary

Select from the drop-down list which of the salaries defined on the
Salary Tab to use in the definition of member’s contributions.

## Additional Cont. Rate (%)

Where contribution rates vary by member, select from the drop-down list
the data item containing the Additional Contribution Rate for each
member. Enter the data as a percentage i.e. for 5% enter `5` and not `0.05`.

## ROC In Service Interest (% p.a.)

This is the rate at which member’s contributions will be increased while
in service. It will only be required if you have selected _Member’s
Contributions_ or _Money Purchase Underpin_ in the [_Return of
Contributions_](actives_basis+disrct.md) field on the Death Cash tab.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## ROC In Deferral Interest (% p.a.)

This is the rate at which member’s contributions will be increased while
in deferment. It will only be required if you have selected a _Member’s
Contributions_ or _Money Purchase Underpin_ in the [_Return of
Contributions_](actives_basis+disrct.md) field on the Death Cash tab.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Company Contributions Definition

Select from the drop-down list the Global Contribution Definition that
contains the company’s contribution parameters. This will only be used
in the Analysis of Surplus module.

The Global Contribution Definition will contain the Method to calculate
contributions and any additional parameters required to define the
contributions.

To add a new Global Contribution Definition use the _Edit Contribution_
Definition button at the bottom of this tab.

For more information please see the Infocus Document relating to Setting
Up Contribution Definitions.

## Ratio of Member Conts

Where Company Contributions are a ratio of the Member Contributions,
enter the ratio. This will only be used in the Analysis of Surplus
Module.

## Use Exact Age in Contributions calculations

Check this box to use the Exact Period of Future Service in the
calculation of the Future 1% of Salaries and Future Member
Contributions. Leave this box unchecked to use future service determined
from age nearest at the valuation date.

Note that when using this option, for consistency with the benefits, the
long/short year of service will be the year prior to NRA if aged less
than NRA or the year after NRA if aged NRA nearest or older.

Some fields are only available to some users.

## Company Conts Salary

Select from the drop-down list which of the salaries defined on the
Salary Tab to use in the definition of company contributions.

## Additional Cont. Rate (%)

Where company contribution rates vary by member, select from the
drop-down list the data item containing the Additional Company
Contribution Rate for each member. Enter the data as a percentage i.e. for
5% enter `5` and not `0.05`. This will only be used in the Analysis of
Surplus Module.

## Current Cost Company Contribution Rate - Death

Enter the Company Contribution Rate in respect of the insured cost of
Death benefits. This will only be used in the Analysis of Surplus
Module.

## - Ill-Health

Enter the Company Contribution Rate in respect of the insured cost of
Ill-health benefits. This will only be used in the Analysis of Surplus
Module.

## Benefits Underpinned

Check this box to value an Underpin to the benefits. Leave unchecked if
the benefits are not underpinned.

## Underpin Contributions Definition

Select from the drop-down list the Global Contribution Definition that
contains the underpin contribution parameters.

The Global Contribution Definition will contain the Method to calculate
contributions and any additional parameters required to define the
contributions.

To add a new Global Contribution Definition use the _Edit Contribution
Definition_ button at the bottom of this tab.

## Underpin Contributions Salary

Select from the drop-down list which of the salaries defined on the
Salary Tab to use in the definition of the Underpin contributions.

## Additional Cont. Rate (%)

This field can be used to value a member specific additional
contribution rate to be included in the Underpin amount.

Select from the drop-down list the data item containing the appropriate
data. The data item should be entered as a percentage i.e. for 5% enter `5`
not `0.05`.

## Initial Underpin Amount

Select from the drop-down list the data item containing the value of the
member’s underpin fund as at the valuation date.

## Underpin Commencement Date

If the Benefits Underpinned box is checked, and for deferreds only the
[Include in Underpin](deferreds_basis+undind.md) on the PUPs is set to
`Split According to Service`, then enter a Start Date for the Underpin
in DD/MM/YYYY format. If the Underpin has always applied simply enter a
date eg 01/01/1900 to ensure that all benefits are compared with the
Underpin.

**Actives** The user should select on each Slice whether or not the
benefits calculated should be compared to the Underpin calculated. The
Start Date for actives will also be used to determine the amount of GMP
to be included in the Underpin comparison. In determining the amount of
GMP included SuperVal will take account of:

-   Pre-88 GMP accruing between 6/4/1978 and 5/4/1988
-   Post-88 GMP accruing between 6/4/1988 and 5/4/1997. (Note 5/4/1997
    will always be used instead of the `Not After Date` on the `Offset
    Slice`.)

**Deferreds** Please note the standard data item `ACW` will always be
used as the value of the underpin fund as at the valuation date. No
other data item can be specified for the underpin for Deferreds.

## Underpin Interest (% p.a.)

For actives, the Underpin Comparison is made at the earlier of Death,
Withdrawal, Early and Normal Retirement. For deferreds, the Underpin
Comparison is made at the earlier of Death, Early and Normal Retirement.
This is the rate at which the underpin fund is increased while the
member remains in service/deferment.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

## Edit Contributions Definition

Clicking the _Edit Contributions_ button allows you to edit a contribution
definition.

Select from the drop-down list the Contribution Definition you wish to
edit.

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