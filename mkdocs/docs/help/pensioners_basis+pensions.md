# Pensioners Basis: Pensions



## Pension Description

Up to 16 separate Pension Benefits can be specified.

Enter a description for the pension or cash benefit being valued eg
Post-97 pension.

This description will appear on the results output.

## Cash Sum or Pension

Select from the drop-down list how to value the benefit. The options
are:

-   Cash
-   Pension

## Pension Amount

Select from the drop-down list the data item to be valued.

## Spouse's Reversion %

This field is used in the Pensioners Module to determine both the
proportion of the member’s pension payable on death after retirement and
death in deferment.

Input the spouse’s reversion factor as a percentage i.e. for 50% enter `50`
rather than `0.5`. If the pension is a single life pension then this
parameter should be set to 0%.

If the spouse’s pension varies by member, this field should be left
blank, and the relevant data item entered into [Spouse’s Pension
Amount](#pensioners_basis+spendata).

## Spouse's Pension Amount

If the spouse’s pension varies by member then select from the drop-down
list the data item containing the amount of the spouse’s pension. If the
spouse’s pension is an identical percentage of the member’s pension for
all members then leave this field blank and enter the percentage in the
[Spouse’s Reversion](#pensioners_basis+warfrac) field.

## Adjustment Factor

A negative or positive loading can be applied to the pension data item.

Enter the number as a multiplier i.e. `1.1` for a 10% increase or `0.9` for a
10% decrease. If no adjustment is required enter `1`. If `0` is entered the
liability for the pension will be zero.

This field can be used to allow for any contingencies, such as
children’s pensions, which are not valued by SuperVal.

## Benefit Commencing Age

This is used to defer the start date of a pension until a point in the
future.

Enter the age at which the pension will commence. For example, a pension
may become payable from SPA. In this case SPA would be the Benefit
Commencing Age.

Any remaining guarantee period calculated is based solely on the data
contained in the data item Date Pension Commenced and not on the age
entered here.

To value an immediate pension either leave blank or enter `0`.

## Pension Ceasing Age

This can be used to stop payment of a pension early.

Enter the age at which the member’s or spouse’s pension payments will
cease. For example, a temporary pension may be payable between
retirement age and SPA. In this case SPA would be the Benefit Ceasing
Age.

Enter 120 if the pension is payable for life. (This represents the end
of the mortality table.)

## Payable on Death in Deferment

If the Benefit Commencing Age is set, the user can specify whether or
not a benefit is paid on death prior to this age. Check this box if this
benefit is payable on death in deferment. Leave the box unchecked if no
benefit is payable.

## Revaluation in Deferment

If the [Benefit Commencing Age](#pensioners_basis+bage) is set, this
is the rate at which the pension will increase between date of valuation
and Benefit Commencing Age.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Pension Increases in Payment

This is the rate at which the pension will increase in payment.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Pension Increases Only

Check this box to value the pension increases on a pension only.

This can be used where annuities have been purchased for pensioners but
`ex-gratia` pension increases are paid from the fund.

## Spouse's Reversion Only

Check this box if you wish to value the spouse’s reversion only.

This can be used when either the entire member’s pension has been
commuted and only the liability for the contingent spouse’s reversion
remains or where separate data items are available for the single life
and the reversionary pension.

## Include in Adjustment at SPA/Death

This option is only available if the [Reduce Pensions at
SPA](pensioners_basis+puprdn.md) box on the Legislation Tab has been
checked.

Check this box if the pension defined is to be included in the
adjustment when the GMP comes into payment at SPA or Death. The user
will then be required to enter the underlying GMP data on which to base
these calculations.

## Pension at Retirement

If the option to [Reduce Pensions at SPA](pensioners_basis+puprdn.md)
has been checked enter the data item containing the pension at `Date
Pension Commenced` that corresponds to the current Pension Data Item
being valued.

This is used to determine the pension increases given on the pension
since retirement for (full) franking of GMP revaluations at SPA or
death.

## Pre 1988 Included at Retirement

If the option to [Reduce Pensions at SPA](pensioners_basis+puprdn.md)
has been checked, and you are not using the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) option, enter the data item
containing the Pre-1988 GMP at retirement underlying the current Pension
Data Item being valued.

If the data is not available, then check the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) box on the Legislation Tab.
However data items containing the total GMP included in the pensions at
Valuation Date and Retirement Date will still be required.

The member may have left active service before retiring and not yet
reached SPA. Therefore the GMP included in the pension may not yet
include revaluation from date of leaving.

## Post 1988 Included at Retirement

If the option to [Reduce Pension at SPA](pensioners_basis+puprdn.md)
has been checked, and you are not using the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) option, then enter the data item
containing the Post-1988 GMP at retirement underlying the current
Pension Data Item being valued.

If the data is not available, then check the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) box on the Legislation Tab.
However data items containing the total GMP included in the pensions at
Valuation Date and Retirement Date will still be required.

The member may have left active service before retiring and not yet
reached SPA. Therefore the GMP included in the pension may not yet
include any revaluation from date of leaving.

## Pre 1988 Included at Valuation Date

If the option to [Reduce Pension at SPA](pensioners_basis+puprdn.md)
has been checked, and you are not using the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) option, then enter the data item
containing the Pre-1988 GMP at retirement included in the Pension at
Valuation Date for the Pension being valued.

If the data is not available, then check the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) box on the Legislation Tab.
However data items containing the total GMP included in the pensions at
Valuation Date and Retirement Date will still be required.

The member may have left active service before retiring and not yet
reached SPA. Therefore the GMP included in the pension may not yet
include any revaluation from date of leaving.

## Post 1988 Included at Valuation Date

If the option to [Reduce Pension at SPA](pensioners_basis+puprdn.md)
has been checked, and you are not using the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) option, then enter the data item
containing the Post-1988 GMP at retirement included in the Pension at
Valuation Date for the Pension being valued.

If the data is not available, then check the [Use Approximate GMP
Ratio](pensioners_basis+gmpsplit.md) box on the Legislation Tab.
However data items containing the total GMP included in the pensions at
Valuation Date and Retirement Date will still be required.

The member may have left active service before retiring and not yet
reached SPA. Therefore the GMP included in the pension may not yet
include any revaluation from date of leaving.

## Male PPF NRA

## Female PPF NRA

On the Legislation Tab, enter the NRA to be attached to the GMP, which
is converted in to excess pension, for PPF valuations.

Elsewhere, for Actives and Deferreds, select from the drop-down list
which of the previously defined PPF NRAs applies to the pension or
benefit slice. The PPF NRAs are specified on the PPF/Cap Tab.

For Pensioners enter the normal retirement age to be used as the PPF NRA
in the PPF (S179 Levy) Valuation. The PPF NRAs are only used to
determine the level of capping required. They do not override the
Benefit Commencing Age. To allow for ill health retirements, use a
sufficiently low age so that all members exceed this age i.e. 16. To allow
for early retirement pensions, use an age such as 50.

## PPF Service Period

PPF guidance, requires the user to show separately the Pre-1997 pension,
post 6 April 1997 to 5 April 2009 pension and the Post 6 April 2009
pension.

Select from the drop-down list whether the pension is:

-   Pre-97
-   97 to 09
-   Post-09

## PPF Revaluation in Deferment

This field can be used to override the Revaluation in Deferment specified for deferred pensions in a PPF S179 (Levy) valuation.

Select from the dropdown list the Global Financial Parameter that contains the rate applicable.  Once selected, the current value of the Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_ button at the bottom of this tab.

## Benefit Included in Cap

Check this box if the pension should be included in the comparison with
the Compensation Cap on a PPF S179 (Levy) Valuation Run.

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

## Add Pension

Clicking on the _Add Pension_ button allows you to add another Pension
definition.

Select whether to use the default pension definition or one of the
existing Pension definitions as the starting point.

## Insert Pension

Clicking on the _Insert Pension_ button allows you to insert another
Pension definition.

Select from the list of Pensions the pension definition you want to
insert the new pension before.

## Edit Pension

Clicking on the Edit Pension button allows you to edit an existing
Pension definition.

You must select the Pension definition to be edited, unless a Pension
definition is currently highlighted, in which case this Pension
definition will be edited.

## Delete Pension

Clicking on the _Delete Pension_ button allows you, after confirmation, to
delete a Pension definition.

You must select the Pension definition to be deleted, unless a Pension
definition is currently highlighted, in which case this Pension
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