# Bulk Annuity: Payment



## Primary Annuitant:  Start Age (x)

## End Age

Enter the start age at which annuities are to be calculated (expressed
in terms of the primary annuitant’s age).

## Guarantee Period (years)

Enter the period for which the member’s pension is guaranteed to be paid
irrespective of whether the member survives this period. For a 5 years
post retirement guarantee enter `5`. If no guarantee is payable enter `0`.

For Pensioners the remaining years guarantee period will be calculated
using the member’s standard data item `DPC - Date Pension Commenced`.

## Overlap on Death in Guarantee Period

If the member’s pension is guaranteed, then the option to select how the
guarantee is paid becomes available.

Check this box if, on the member’s death during the guarantee period,
all outstanding payments in the guarantee period are paid as a lump sum
at death and any spouse’s reversion becomes payable immediately. When
valuing Actives or Deferreds or using the annuity calculators, the
option to select whether this benefit is discounted or undiscounted
becomes available. For Pensioners, the lump sum is calculated as the sum
of the undiscounted payments at the point of death when this option is
selected.

Leave this box unchecked if, on the member’s death during the guarantee
period, payments continue until the end of the guarantee period and any
spouse’s reversion becomes payable thereafter. Payments are always
discounted in this scenario.

## Discounted LS on Death in Guarantee Period

The field is used to specify whether the Lump Sum paid as a result of a
guarantee after death is discounted or undiscounted for Actives,
Deferreds and the Annuity Calculator.

Check this box to discount, with interest, the lump sum payable. Leave
this box unchecked if the lump sum payable is undiscounted.

## Deferment Age

Specify the Deferment Age (if any) in years (expressed in terms of the
age of the primary annuitant). This will be after the start age for the
annuitant.

## Ceasing Age

The age at which annuity payments will cease in years (expressed in
terms of the age of the primary annuitant).

The maximum allowable age of 120 will include payments for the life of
the primary annuitant (and reversionary payments, if any, for the life
of the reversionary annuitant).

## Payment Frequency

Select from the drop-down list the frequency of the pension payments.
The options are:

-   Annual
-   Semi-Annual
-   Quarterly
-   Monthly
-   Lunar-Monthly
-   Fortnightly
-   Weekly
-   Continuous

## Payment Mode

Select from the drop-down list the timing of pension payments. The
options are:

-   In Arrears
-   In Advance

## Proportions Married Table

Double click to select the table containing the proportion married for
members at each age.

In ongoing runs, these fields are used to determine the proportion of
the member’s benefit paid to a spouse or partner on death in service
(actives only), death in deferment or death after retirement. The field
[Spouse’s Definition](bases+spmethod.md) enables you to select how the
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

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Proportion Married

Users can express the proportion married as a single percentage across all ages.

## Spouse's Age Difference (x-y)

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

## Spouse's Reversion

Enter the reversion payable to the spouse (if any) expressed as a
percentage of the member’s annuity.

## Reversion payable to Spouse on Death in Deferment

If there is a deferment period, check the box to include in the
calculation a reversionary annuity payable to the spouse on the death of
the member during that deferment period.

## Value Spouse's Reversion only

Check this if the annuity for only the Spouse’s Reversion is required.

## Interest Rate (% p.a.)

This is the annual rate at which benefits will be discounted.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field. When
using the annuity calculators, a fixed value may also be entered i.e. 9
for 9.00%.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Specify a Different Rate of Return on Reinvestment while in Deferment

## Reinvestment Rate in Deferment (% p.a.)

Check this box to allow for a different rate of return on the
reinvestment of investment earnings during the period of deferment.

You will then be required to enter a Reinvestment Rate in Deferment.
This will be used to determine a `modified` discount rate for this
period.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Revaluation in Deferment (% p.a.)

This is the annual rate of increase in the benefit during the deferment
period.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Pension Increases in Payment (% p.a.)

This is the annual rate of increase in the pension once in payment.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Value Pension Increases only

Check this if the annuity for only the Pension Increases is required.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

## Run

Click the _Run_ button to run the calculations.

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