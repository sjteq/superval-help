# Deferreds Basis: Financial



## Pre Retirement Interest Rate

This is the annual rate at which benefits will be discounted pre
retirement.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

For Active members, the user can select whether the Pre Retirement
Interest Rate or the Post Retirement Interest Rate is used for Accrued
Valuations and for discounting benefits post withdrawal in the
[Switch](actives_basis+swindic.md) field.

## Post Retirement Interest Rate

This is the annual rate at which benefits will be discounted post
retirement.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

For Active members, the user can select whether the Pre Retirement
Interest Rate or the Post Retirement Interest Rate is used for Accrued
Valuations and for discounting benefits post withdrawal in the
[Switch](actives_basis+swindic.md) field.

## Excess Revaluation

This is the rate at which the PUP will increase in deferment i.e. between
valuation date and NRA.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value is shown
to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Count Complete Years

Check this box if exits before NRA should only receive revaluations for
each complete year between valuation date and date of exit. Leave the
box unchecked to allow for the extra half-year revaluation to date of
exit.

Exits before NRA, such as early retirement and death in deferment, are
assumed to occur half-way through the year i.e. 0.5, 1.5, 2.5 years after
the valuation date. By checking this box, these benefits will receive
revaluations for the number of complete years only i.e. 0, 1, 2. If the
box is unchecked, the benefits will receive an additional half-year of
revaluation i.e. 0.5, 1.5, 2.5.

On each of the PUPs, Ind PUPS and NSPUPs Tabs you can choose to override
this entry and use the other approach.

## NRA Exits Rounding

Select from the drop-down list how the rounding for exits at NRA should
be calculated. The revaluation of the PUP to Normal Retirement Age will
be based on the exact duration between Valuation Date and Normal
Retirement Date, rounded according to the parameter entered. The options
are:

-   Exact Days
-   Months Rounded Down
-   Nearest Months
-   Months Rounded Up
-   Years Rounded Down
-   Nearest Years
-   Years Rounded Up
-   Complete Tax Years

The discounting of the benefit will be based on years nearest.

## Pre Valuation Date Revaluation

Select from the drop-down list how to revalue the excess pension between
date of leaving and valuation date. The options are:

-   No
-   Fixed Rate
-   s52 index

Use `No` where the excess pension already includes revaluations to the
valuation date.

Use `Fixed Rate` where a single rate of revaluation applies between date
of leaving and date of valuation. The value can then be entered in the
[Pre Valn Date Rate.](#deferreds_basis+pastrevn)

Uses `s52 Index` where a table of revaluation rates between date of
leaving and date of valuation should be applied. The table can be
entered in the [Pre Valn Date Factor Set](#deferreds_basis+revset).

## Pre Valuation Date Factor Set

Select from the drop-down list the appropriate Factor to use. This
option is available if [Pre Valn Date
Revaluation](#deferreds_basis+pastrev) is set to s52 Index.

## Pre Valuation Date Rate

Pre Valn Date Rate

This is the rate at which the excess pension will be increased between
date of leaving and date of valuation if Fixed Rate has been selected
for [Pre Valn Date Revaluation](#deferreds_basis+pastrev).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Pre Valuation Date Rate Rounding

Where `Fixed Rate` has been selected for [Pre Valuation Date
Revaluation](#deferreds_basis+pastrev), select from the drop-down
list how the rounding for revaluations between date of leaving and
valuation date should be calculated. The options are:

-   Exact Days
-   Months Rounded Down
-   Nearest Months
-   Months Rounded Up
-   Years Rounded Down
-   Nearest Years
-   Years Rounded Up
-   Complete Tax Years

## Pre 1988 GMP

This is the rate at which Pre-1988 GMP benefits will increase in payment
annually.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Post 1988 GMP

This is the rate at which Post-1988 GMP benefits will increase in
payment annually.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Main

This is the rate at which pensions will increase in payment annually
where Main has been selected for Pension Increases in Payment on either
the Slices tab (Active) or one of the PUPS tabs (Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Special

This is the rate at which pensions will increase in payment annually
where Special has been selected for [](bases+dynind.md) Pension
Increases in Payment on either the Slices tab (Active) or one of the
PUPS tabs (Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## PenInc3

This is the rate at which pensions will increase in payment annually
where Pension Increase 3 has been selected for Pension Increases in
Payment on either the Slices tab (Active) or one of the PUPS tabs
(Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## PenInc4

This is the rate at which pensions will increase in payment annually
where Pension Increase 4 has been selected for Pension Increases in
Payment on either the Slices tab (Active) or one of the PUPS tabs
(Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Timing of Pension Increases

Select from the drop-down list how the timing of pension increases
should be applied. The options are:

-   Continuous
-   Review Date

If Review Date is selected then enter the day and month (DD/MM) the
increase is paid in the [Increase Date](#bases+incdat) field.

## Increase Date

If the [Timing of Pension Increases](#bases+incind) has been set to
Review Date then enter the day and month of the pension increase date.
The date should be in DD/MM format.

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