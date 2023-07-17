# Actives Basis: Salaries



## Salary Description

Describe the salary being defined i.e. Basic Salary – 1yr ave.

This name will be used throughout the basis file when selecting which
salary to use.

## Initial Salary

Select from the drop-down list the data item containing the salary to be
used within this salary definition.

This would typically be the data item containing the (pensionable)
salary as at the valuation date. It could be either of the standard
data item Current Salary or Previous Salary or one of the numeric
non-standard data items.

If the actual Final Pensionable Salary data item (including averaging)
at the valuation date is available then this should be entered into the
[Initial Final Average Salary](#actives_basis+fasdata) field.

## Override Salary Increase Rate

The user has the option to enter an override for the salary increase
rate for the current Salary definition.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

If left blank the Overall Salary Increase Rate on the Financial tab will
be used.

## Post NRA Salary Revaluation Rate

The user has the option to override the salary increase assumption for
members who retire after NRD. This field is only used if _NRA Salary_ is
selected in the [Salary for Late Retirement](actives_basis+lrsalary.md)
on the Late Retirement tab and only applies to the salary definition
selected.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

If left blank the [Overall Salary Increase
Rate](actives_basis+salinc.md) on the Financial tab will be used.

Note: Not all functionality is available to all users.

## Adjustment Factor

This field is a loading adjustment for the salary.

This option could be used where the member data was out of date and
needs to be increased to take account of an extra half year of salary
inflation. The multiplier could be set to `1.04` if salary increases were
at 8% p.a.

## Male Promotional Scale Table

## Female Promotional Scale Table

Promotional salary scales are salary increases that are provided in
addition to the general salary increases previously specified.

Double click to select from either an age related promotional salary
scale (`S` Type) or a service related promotional salary scale (`ST`
Type). For both types, the table will contain the year on year rates
(and not cumulative rates).

When using a service related promotional scale the user will be required
to input the date from which service will be calculated in the [Date for
Durational Decrements](actives_basis+durndate.md) field on the
Demographic Tab.

General salary increases are normally specified in the [Salary
Increase](actives_basis+salinc.md) field on the Financial Tab.
Alternatively, for a particular salary definition this can be overridden
by the [Salary Increase Override](#actives_basis+salinf) on the
Salaries Tab.

Some options are only available to some users.

## Timing of Salary Increases

Select from the drop-down list the timing of salary increases. The
options are:

-   Review Date
-   Continuous
-   Weighted

If `Review Date` is selected, salaries will be updated on the date
entered in Review Date.

If `Continuous` is selected, salaries will be increased continuously.

If `Weighted` is selected, salaries will be updated on the date entered
in Review Date but weighted when calculating Final Average Salary.

The projection of Salary is the same for both Review Date and Weighted.

The difference relates to the calculation of Final Average Salary. Under
Review Date, Final Average Salary is the average salary as at the last N
review dates. Under Weighted, Final Average Salary is the average salary
over the last N years. Hence, Review Date can be used to model Final
Average Salaries that only increase once a year on the Review Date
whereas Weighted is used to model Final Average Salaries that increase
continuously during the year.

For more information on how these different salaries are calculated
please see the Infocus Document relating to Salary Projections in
SuperVal.

## Review Date

If Salary Increase Timing was either `Review Date` or `Weighted` then
enter the date salaries increase in the form DD/MM.

## Averaging Period

Enter the number of years over which salaries are averaged either on
leaving or at retirement.

## Averaging Ceases

Select from the drop-down list when the salary averaging should be
applied. The options are:

-   On Leaving Service
-   At NRD

Under `On Leaving Service` the salary averaging will be applied on all
decrements.

Under `At NRD` the salary averaging will only be applied on exit at
Normal Retirement Date.

## Initial Final Average Salary

Select from the drop-down list the data item containing the initial
Final Average Salary.

This will be used as Final Average Salary as at the valuation date and
blended with projected final average salary calculated using Current
Salary and Salary Inflation to produce Final Average Salary during the
specified averaging period.

If left blank, Final Average Salary as at the valuation date will be
calculated using Current Salary deflated using the Salary Inflation rate
specified.

More information on the application of this field can be found in the
Infocus Document relating to Salary Projections.

## Last Salary in Average

Check this box if the last salary should be included in the final
average salary calculation. Leave unchecked to exclude the last salary
in the final average salary calculations.

If checked, SuperVal will average the salary over the averaging period
specified. If unchecked, SuperVal will add 2 years to the averaging
period specified.

## Deduction Initial Value

Enter the amount of salary deduction you wish to apply. This can either
be a fixed amount for all members or a member specific amount.

To use a fixed value across all members, enter the value here. To use a
member specific value, select from the drop-down list the appropriate
data item.

For example, if the pensionable salary definition is reduced by the
Lower Earnings Limit, enter the Lower Earnings Limit as at the valuation
date in this field.

If both a maximum and a deduction are used, then the maximum is applied
before the deduction i.e. entering a maximum of Upper Earnings Limit and
deduction of a Lower Earnings Limit would give Band Earnings.

## Deduction Adjustment Factor

This field allows the user to adjust the deduction by a fixed factor. It
might be used where the data used for the deduction is out of date and
needs to be increased to take account of an extra part year of
inflation.  
Enter the number as a multiplier, e.g. `1.1` for a 10% increase or `0.9` for
a 10% decrease. For no adjustment enter a value of `1`.

This field can also be used to add the deduction amount on to the
salary. To do this ensure the value entered is negative i.e. `-1` to add the
deduction, without adjustment, onto the salary.

## Deduction Increase Rate Override

This the rate at which the deduction will be increased.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

If the Deduction is non-increasing select a Global Financial Parameter
set to 0.

If this field is left blank, SuperVal will use the [Salary Overall
Parameters Increase Rate](actives_basis+salinc.md) specified on the
Financial tab.

## Maximum Initial Value

Enter the amount of salary maximum you wish to apply. This can either be
a fixed amount for all members or a member specific amount.

To use a fixed value across all members, enter the value here. To use a
member specific value, select from the drop-down list the appropriate
data item.

For example, if the pensionable salary definition is restricted by the
Earnings Cap, then enter the Earnings Cap as at the valuation date in
this field.

If both a maximum and a deduction are used, then the maximum is applied
before the deduction i.e. entering a maximum of Upper Earnings Limit and
deduction of a Lower Earnings Limit would give Band Earnings.

## Maximum Adjustment Factor

This field allows the user to adjust the maximum by a fixed factor. It
might be used where the data used for the maximum is out of date and
needs to be increased to take account of an extra part year of
inflation.  

Enter the number as a multiplier, e.g. `1.1` for a 10% increase or `0.9` for
a 10% decrease. For no adjustment enter a value of `1`.

## Maximum Increase Rate Override

This the rate at which the maximum will be increased.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

If the maximum is non-increasing select a Global Financial Parameter set
to 0.

If this field is left blank, SuperVal will use the [Salary Overall
Parameters Increase Rate](actives_basis+salinc.md) specified on the
Financial tab.

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

## Add Salary

Clicking on the _Add Salary_ button allows you to add another Salary
definition.

Select whether to use the default salary definition or one of the
existing Salary definitions as the starting point.

## Insert Salary

Clicking on the _Insert Salary_ button allows you to insert another Salary
definition.

Select from the list of salaries the salary definition you want to
insert the new salary before.

## Edit Salary

Pressing the _Edit Salary_ button allows you to edit a salary definition.

You must select the Salary definition to be edited, unless a Salary
definition is currently highlighted, in which case this Salary
definition will be edited.

## Delete Salary

Clicking the _Delete Salary_ button allows you to, after confirmation,
delete a Salary definition.

You must select the Salary definition to be deleted, unless a Salary
definition is currently highlighted, in which case this Salary
definition will be deleted.

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