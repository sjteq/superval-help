# Batch Define



## Valuation Method

The required Valuation Method should be selected first.

## Saved Bases

Select the Basis Parameter Set (or Sets) to be batched. Only the Basis
Parameter sets from the selected Basis Parameter File which are
appropriate for the Valuation Method selected will be presented.

## Sex Selection

Select from the drop-down list which sexes to include in the valuation
run. The options are:

-   Both
-   Males
-   Females

## Test Valuation Run

Select from the drop-down list what output to receive. The options are:

-   No
-   Limited
-   Full

Use `No` to value all members. No Varprints will be produced.

Use `Limited` to value members that have been `starred` in the data
file. The output will include results at every fifth age.

Use `Full` to value members that have been `starred` in the data file.
The output will include results are every age.

## Interpolated Exact Age Results

If Interpolated Exact Age Calculations are required please tick this
box.

SuperVal can do more accurate valuation calculations by interpolating
between results at age last exact and age next exact (allowing for the
members exact age in years including fractional part in days).

## Aggregate Benefits before Valuing

Check this box to aggregate the benefits of members of the same age
before valuing. This will speed up the valuation process.

## Control Period

A Control Period (expressed in years) is required for either the
Projected Unit Credit or the Defined Accrued Benefit valuation methods.

For the Projected Unit Credit method, enter the period over which the
`Normal Cost` will be calculated.

For the Defined Accrued Benefit method, enter the period over which
funding towards the target Accrued Benefit is achieved. (Please note
this can also be modified when consolidating these runs.)

## Insured Benefits in Normal Cost

For the Projected Unit Credit methods, specify whether you wish the cost
of the insured benefits to be included in the `Normal Cost`.

## Target Accrued Benefit

For the Defined Accrued Benefit method, select from the drop-down list
which of the Accrued Benefits is to be used as the target Accrued
Benefit. The options are:

-   Past Service Liability
-   Discontinuance Benefits

## New Entrant Model Replacement

You must specify whether you wish the new entrant model replacement
projection to be carried out.

This will be carried out immediately following the completion of the
valuation run. It is possible to fit alternative new entrant models
later using the saved valuation results.

## New Entrant Model Parameters

If the new entrant model replacement option is selected, you must select
the New Entrant Model Parameters to be used for the projection.

## Valuation Date

The valuation can be carried out at either the Previous or the Current
Valuation Date (as defined in the Scheme Details).

## Analysis of Surplus

Check the box if you require Analysis of Surplus calculations to be
carried out.

## Cap Accrued Benefits

For actives or deferreds ongoing runs, the user has the option of
Capping the Accrued Benefits in line with the Cap for the PPF Protection
Fund. Check the box to apply the PPF Benefit Cap to the Accrued
Benefits.

The PPF Benefit Cap will increase at the assumption specified in the Cap
Increases before/after Discontinuance specified in the PPF Global
Parameters.

## S143 Entry Valuation

When running a Deferreds Pension Protection Fund valuation, check this
box to use the S143 PPF Entry Valuation methodology

## Store Results for Consolidation

Check this box if you would like SuperVal to produce the valuation
results within the Excel File and to store these for consolidating at a
later date.

Leave this box unchecked to produce the text output only.

You may wish to leave this unchecked until you have completed the
initial checking of the valuation results. The valuation can then be
re-run and the consolidation output stored. Once selected, the results
of the run for each category will be written to database that will be
located in the Consolidation folder specified.

## ALM/LDI Interface Required

If you have the additional module containing the ALM/LDI functionality,
then check the box if you wish these results to be stored.

## Summarise All Results by Age

To reduce the size of the valuation output file, the individual member
results can be summarised (or grouped) by age. Check this box to produce
summarised output containing just two lines of output for each age group
valued. (One line each for males and females.)

## Individual Member Cash Flows

Select this field if individual cashflows are required. The individual
cashflows will be displayed in the MemberResults Table in the database.

## Output Valuation Factor Tables

Select this field if you want the Valuation Factor tables to be written in the
Excel output and the database.

## Input Data File in Text Output

Select how much of the input data file output should be printed in the
valuation output file. The options are:

-   Limited
-   None
-   All

If Limited is selected, the first two pages of data will be printed.

## Consolidate Member Results

This field only affects the results shown in the Text Output for a
pensioners run. If unchecked, the output file will show the liability
for each pension for each member separately. If checked, the output file
will summarise all of the pensions for each member into one line of
output.

## Export Individual Member Results

Indicate if you wish to export a CSV file of individual member results
as part of the valuation run.

## OK

When you have finished entering the relevant information, click the _OK_
button to move to the next screen.

SuperVal will check that all of the required entries on the page have
been made. If additional fields require data SuperVal will show briefly
in red which is the first of these fields found on the page.

## Cancel

Clicking on the _Cancel_ button allows you to return to the previous
screen without saving any of your changes.