# Actives Basis: Financial



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
[Switch](#actives_basis+swindic) field.

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
[Switch](#actives_basis+swindic) field.

## Switch

This field is used to determine which of the Pre Retirement Interest
Rate or the Post Retirement Interest Rate is used for discounting post
withdrawal and for Accrued Valuations. Select from the drop-down list
which of the following options to use:

-   Use Post-Ret Int for Accrued/Wdls
-   Use Pre-Ret Int for Accrued/Wdls

The table below sets out which interest rate is used for each of the
decrements under both scenarios.

Ongoing Valuation      | Using Pre Ret Int Rate | Accrued Using Pre Ret Int Rate | Ongoing Valuation Using Post Ret Int Rate | Accrued Using Post Ret Int Rate
-----------------------|------------------------|--------------------------------|-------------------------------------------|--------------------------------
**Retirement Pensions** |
- Pre Retirement       | Pre  | Pre  | Pre  | Post
- Post Retirement      | Post | Post | Post | Post
**Leaving Service Pension** |
- Pre Exit             | Pre  | n/a  | Pre  | n/a
- Exit to Retirement   | Pre  | n/a  | Post | n/a
- Post Retirement      | Post | n/a  | Post | n/a
**DIS Lump Sum**       | Pre  | n/a  | Pre  | n/a
**DIS Spouse&rsquo;s** |
- Pre death            | Pre  | n/a  | Pre  | n/a
- Post death           | Post | n/a  | Post | n/a
**DID Lump Sum** |
- Pre exit             | Pre  | Pre  | Pre  | Pre
- Exit to death        | Pre  |      | Pre  |
**DID Spouse&rsquo;s** |
- Pre Exit             | Pre  |      | Pre  |
- Exit to Death        | Pre  | Pre  | Pre  | Pre
- Post Death           | Post | Post | Post | Post

## Salary Increase Rate

This is the annual rate at which salaries for all members will increase
to date of exit. A [Promotional Salary Scale](actives_basis+sxx.md) in
excess of general salary increases can be specified on the Salaries tab.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

This will be used in all salary definitions unless the [Salary Inflation
Rate Override](actives_basis+salinf.md) on the Salaries tab is
populated.

## Revaluation Rate

This is the annual rate at which CARE benefits will be increased to date
of exit.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## First year of CARE accrual is revalued immediately

Check this box to revalue the CARE benefit accrued in the year of exit
immediately. Leave this box unchecked to revalue the CARE benefit
accrued in the year of exit in the following year only. Consider a
member with:

P = Accrued CARE Pension  
S = Salary over the year  
r = Revaluation Rate.

The accrual rate is 1/60.

If the box is checked to increase the accrued benefit immediately then
the benefit at the end of the year is calculated as (P + S/60) &times; (1+r)

If the box is unchecked then the benefit is calculated at the end of the
year as $P \times (1+r) + S/60$

Not all fields are available to all users.

## Timing of Revaluations

Select from the drop-down list how to apply CARE Scheme Revaluations.
The options are:

-   Continuous
-   Review Date

If Review Date is selected then enter the day and month (DD/MM)
Revaluations are reviewed in the [Review Date](#actives_basis+revdat)
field.

## Review Date

If CARE Scheme Revaluations take place on a Review Date, then enter the
review date using the DD/MM format.

## Rate

This is the first of three revaluation rates that can be used to
increase the excess pension between date of exit and Normal Retirement
Age.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Rate 2

This is the second of three revaluation rates that can be used to
increase the excess pension between date of exit and Normal Retirement
Age.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Rate 3

This is the third of three revaluation rates that can be used to
increase the excess pension between date of exit and Normal Retirement
Age.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this Tab.

## Curtate Revaluation Period

Check this box if exits before NRA should only receive revaluations for
each complete year. Leave the box unchecked to allow for the extra
half-year revaluation.

Exits before NRA, such as early retirement and death in deferment, are
assumed to occur half-way through the year i.e. 0.5, 1.5, 2.5 years after
the valuation date. By checking this box, these benefits will receive
deferred revaluations for the number of complete years only i.e. 0, 1, 2.
If the box is unchecked, the benefits will receive an additional
half-year of revaluation i.e. 0.5, 1.5, 2.5.

## Male Barber Adjustment to Main

## Male Barber Adjustment to Special

## Male Barber Adjustment to PenInc3

## Male Barber Adjustment to PenInc4

## Female Barber Adjustment to Main

## Female Barber Adjustment to Special

## Female Barber Adjustment to PenInc3

## Female Barber Adjustment to PenInc4

If you have a withdrawal decrement, the accumulated benefit from the
Slices will be valued at the [Normal Retirement Age](bases+nra.md)
specified on the Membership Tab. The early retirement/late retirement
parameters are ignored.

If part of the accumulated benefit can be taken earlier or later than
NRA, then a loading to that part of the withdrawal liability can be
made. The loading adjustment is applied to the accumulated benefits
arising from all Slices where Early Retirement Reduction Factors 1
(ERF1) has been selected.

The loading can either be fixed or variable. If the loading is fixed
then enter the loading to be applied to the benefit as a multiplier ie
to load the benefits by 20% enter a loading of 1.2. If the loading
varies with the Financial Assumptions used then enter the loading as a
Scheme Constant. (Right click over the field for a list of the constants
that have been defined.)

Different loadings can be applied to the Male and Female benefits and
the benefits arising from each of the 4 different pension increase
rates.

Although SuperVal will not apply early retirement reduction factors to
the different Benefit Slices on withdrawal, it is able to determine
which part of the accumulated benefits arises from Slices with ERF1 and
which part arises from Slices with ERF2. The accumulated benefits
arising from Slices with ERF1 will be multiplied by the loading factor
in these fields.

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