# Deferreds Basis: Membership



## Male Retirement Age Parameter Set

## Female Retirement Age Parameter Set

Retirement Factor Parameter Set is a Scheme Global parameter which
groups the Male or Female Retirement Factor variables. This can be
created by using either the `Create Globals` function or using the
_Add/Edit Retirement Factors_ button. Once created, these parameters
can be edited without going back into the Basis similar to other global
parameter sets.

## Male Normal Retirement Age

## Female Normal Retirement Age

Specify the Normal Retirement Age i.e. the age at which it is assumed
members will retire.

For actives where there is no Late Retirement Age and deferreds, the
decrements specified in the basis will affect the member up to the NRA
specified. On survivorship to NRA, all members will be assumed to retire
on the anniversary of the valuation date. Any withdrawal Pups will be
assumed payable from this age ( i.e. early retirements would be ignored
for withdrawals).

For actives where there is a Late Retirement Age, the decrement
specified in the basis will affect the member up to the LRA specified.
On survivorship to NRA, the proportion of members specified in the ER/LR
decrement will be assumed to retire on the anniversary of the valuation
date. Thereafter members will be assumed to retire on the anniversary of
the valuation date in line with the decrement table specified. On
survivorship to LRA, all members will be assumed to retire. Any
withdrawal Pups will be assumed payable from this age (i.e. early
retirements would be ignored for withdrawals).

State Pension Age (SPA) is automatically set by SuperVal to be 65 for
males and 60 for females. This will be the age at which the GMP will be
assumed to be payable (or NRA if this is later). The interaction between
NRA and SPA is illustrated below:

If NRA is less than SPA:

![](img/bm5.gif)

If NRA is greater than SPA then:

The Pension is immediately broken down in to its components of excess
over GMP, Pre-1988 and Post-1988 GMP. The GMP elements of the pension
will have late revaluation applied. The late revaluation will include
1/7% per week and increases to Post-1988 GMP. The rate at which the
Post-1988 GMP is increased depends on whether Statutory Increases are
applied.

Members who are over NRA (or LRA if specified) will be valued as
follows:


Actives

: Members who are over NRA will be assumed to retire immediately.


Deferreds

: Members who are over NRA will be assumed to retire immediately.

Please see the help for Early-Retirement Factors for how these will be
applied to members over NRA.

Note: The Late Retirement functionality is only available to some users.

## Normal Retirement Date Indicator

Select from the drop-down list how to define Normal Retirement Date for
determining service and final average salary in the actives benefit
calculations and deferred revaluations for the deferreds and active
withdrawals benefit calculations. The options are:

-   Exact Birthday
-   End of Month following Birthday
-   End of Year following Birthday

Note: The discounting of benefits and the selection of decrement rates
will be based on age nearest.

## Date Left Active

If [Fixed Revaluation Rate to SPA](deferreds_basis+gmprev2.md) has been
selected, then select from the drop-down list the data item containing
the date the member left active service.

For Deferreds, the date that members left active service is NOT a
standard data item but a user defined item (prefixed with a `q`). The
standard data item `DOE` will contain the date of exit from deferred
status i.e. transfer out, retirement, death.

## Add/Edit Retirement Ages

Add or Edit any Retirement Age parameter sets.

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