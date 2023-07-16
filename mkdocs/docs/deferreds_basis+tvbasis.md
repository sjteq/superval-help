# Deferreds Basis: TVBasis



## Same as Valuation Basis Cash Flows

## Same as Valuation Basis Interest Rates

## Same as Valuation Basis Increase Rates

## Same as Valuation Basis Spouse Parameters

Transfer assumptions can be set to always be the same as the Valuation Basis i.e. either one or more of the following:

-   cash flow parameters (capitalised or spread)
-   interest rates
-   increase rates
-   spouse parameters (proportion married, age difference)
-   member’s pre retirement mortality
-   member’s post retirement mortality
-   spouse / partner’s post retirement mortality

## Transfer Benefits Capitalised or Spread

This and the other Cash Flow Parameters only affect the `Cash Flow
Summary` page in the Excel Output/Consolidation Output. They do not have
any effect on the Valuation Results.

Select from the drop-down list the option to use. The options are:

-   Capitalise
-   Spread

If `Capitalise` is selected the output will show the cashflows assuming
the benefits are capitalised at the point of first payment.

If `Spread` is selected the output will show the cashflows as they
become due.

However, the Death in Deferment Liability shown will always be the
capitalised value of the payments. The user can choose the point at
which the Death in Deferment Liability is shown in the Cash Flows
summary in the [Death in Deferment Method](actives_basis+didmethod.md)
field.

In addition, if `Spread` is chosen for Actives or Deferreds, the user
will be required to specify at which point the Underpin Liability is
capitalised in the [Underpin Method](bases+umethod.md).

When running a DAB method valuation, this field must be set to
Capitalise.

## Transfers Pre Retirement Interest Rate

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

## Transfers Post Retirement Interest Rate

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

## Transfers Pre 1988 GMP

This is the rate at which Pre-1988 GMP benefits will increase in payment
annually.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Transfers Post 1988 GMP

This is the rate at which Post-1988 GMP benefits will increase in
payment annually.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Transfers Main

This is the rate at which pensions will increase in payment annually
where Main has been selected for Pension Increases in Payment on either
the Slices tab (Active) or one of the PUPS tabs (Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Transfers Special

This is the rate at which pensions will increase in payment annually
where Special has been selected for [](bases+dynind.md) Pension
Increases in Payment on either the Slices tab (Active) or one of the
PUPS tabs (Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Transfers PenInc3

This is the rate at which pensions will increase in payment annually
where Pension Increase 3 has been selected for Pension Increases in
Payment on either the Slices tab (Active) or one of the PUPS tabs
(Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Transfers PenInc4

This is the rate at which pensions will increase in payment annually
where Pension Increase 4 has been selected for Pension Increases in
Payment on either the Slices tab (Active) or one of the PUPS tabs
(Deferred).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Transfers Spouse Parameter Set

Spouse Parameter Set is a Scheme Global parameter which groups the
Spouse variables. This can be created by using either the `Create
Globals` function or using the _Add/Edit Spouse Parameters_ button. Once
created, these parameters can be edited without going back into the
Basis similar to other global parameter sets.

## Transfers Spouse Definition

Select from the drop-down list how to value the spouse’s pension on
death after retirement. The options are:

-   Retirement
-   Death

If Retirement is selected, SuperVal will use the proportion married as
at the member’s age at retirement.

If Death is selected, SuperVal will use the proportion married as at the
member’s age at death.

For more information please see the Infocus Document relating to
Proportion Married.

## Male Transfers Proportion Married Table

## Female Transfers Proportion Married Table

Double click to select the table containing the proportion married for
members at each age.

In ongoing runs, these fields are used to determine the proportion of
the member’s benefit paid to a spouse or partner on death in service
(actives only), death in deferment or death after retirement. The field
[Spouse’s Definition](#bases+spmethod) enables you to select how the
proportion married is applied.

In PPF runs the fields in the Scheme PPF parameters can be used to enter
the proportion married separately for male and female spouses and male
and female partners.

If 90% of members are assumed to be married at all ages then enter a
table containing `0.9`.

More information is available in the Infocus Document called Proportion
Married.

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

## Male Transfers Proportion Married

## Female Transfers Proportion Married

Users can express the proportion married as a single percentage across all ages.

## Male Transfers Age Difference Table (m-f)

## Female Transfers Age Difference Table (f-m)

This field is used to enter an age-dependent table if the age difference
between a member and their spouse varies according to the member’s age.
It is used when valuing death benefits prior to retirement and
contingent annuities on death after retirement. For pensioners death
benefits prior to retirement may occur when the [Benefit Commencing
Age](pensioners_basis+bage.md) is after the member’s current age.

Double click to select the `AD` table that contains the relevant data.
The table should contain the values for Member’s Age minus Spouse’s Age
ie if Members are 3 years older than their spouse enter `3`.

This field is only available to some users.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Male Transfers Age Difference (m-f)

## Female Transfers Age Difference (f-m)

This field is used to set an age difference between a member and their
spouse that is identical for all members. It is used when valuing death
benefits prior to retirement and contingent annuities on death after
retirement. For pensioners death benefits prior to retirement may occur
when the [Benefit Commencing Age](pensioners_basis+bage.md) is after
the member’s current age.

Enter the relevant value containing Member’s Age minus Spouse’s Age ie
if Members are 3 years older than their spouse enter `3`.

If you wish to use an Age Rating that varies with the member’s age then
leave this field blank and the Age Difference Table will become
available. (This functionality is not available for PPF runs or for the
annuity calculators.)

The Age Difference Table field is only available to some users.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

## Add/Edit Spouse Parameters

Add or Edit any Spouse parameter sets.

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