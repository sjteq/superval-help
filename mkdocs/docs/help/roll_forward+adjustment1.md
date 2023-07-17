# Roll Forward: Adjustment1



## Category Selections

Select the list of Categories for these Adjustments

## Fixed Revaluation Rate

Select this box to use Fixed Revaluation Rate for GMP data fields

## Statutory GMP Increases

Select this field to use Statutory GMP Increases for GMP data fields

## Data Field

These are the GMP0 and GMPE0 defined in the data

## Revaluation

Enter the GMP Revaluation Rate

## Increases

Enter the GMP Increase Rate

## Grid Help

Right-clicking on a column heading presents a menu with the following
options which allow you to expand or reduce the number of columns of
data to be entered:

-   Add a new column to the right of the grid;
-   Insert a new column at the position of the cursor; and
-   Delete the current column at the position of the cursor.

## Grid Help

Right-clicking on the Top Left Corner of the grid displays a menu which
allows you to set the following Grid Editing Options:

-   Editing of a cell can be invoked by either clicking on the cell or
    by pressing F2 when the cell is active (Clicking will only change
    the current active cell); and
-   determine the cursor movement once editing is complete to be either
    to the next cell down, the next cell to the right or to stay in the
    current cell.

## Timing of GMP Pension Increases

Select the Timing of GMP Pension Increases

## Increase Date

Specify the Day and Month of the GMP Pension Increase Date

## Data Field

These are the fields that have been brought over from the basis for the
Category selected

## Escalation Type

Select the Escalation Method:


None

: This option will apply no escalation to the Data Field.

: Fields required: None


Interest/Revaluation

: This will perform a simple roll-up at the rate specified in the
‘Escalation Rate’ column for the Roll Forward period.

: Fields required: Escalation Rate

: Where (assumed continuous increases).


Increases

: The method of escalating the data field will depend on which `Escalation Timing` is specified.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`)


Escalation Rate

: If Escalation Timing is Continuous, the same calculation will be applied as in Interest/Revaluation above. If the timing is Review Date, a full year’s increase will be applied on each Review Date within the Roll Forward period.


Inflation

: The same calculation will be applied as for Increases but with the inclusion of any Promotional Salary Increases.

: Fields required: `Salary Scale` (Male and Female), `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Escalation Rate`


Age Dependent

: This method of escalating the data field will depend on the Payment Start Age specified.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Payment Start Age` (Male and Female), `Age Dependent Revaluation`


Age-Dependent Increases

: Revaluation will be applied prior to the Payment Start Age and Increases will be applied after the Payment Start Age. The calculation is described in Revaluation and Increases above.


Excess over GMP

: This calculation is similar to Age Dependent above but allowing for the GMP.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Payment Start Age` (Male and Female), `Age-Dependent Revaluation`


Age-Dependent Increases

: The formula is:


If Not Fixed

: The calculation is applied as for Age Dependent if GMP Fixed Revaluation is not checked. If GMP Fixed Revaluation *is* checked: substitute Fixed Revaluation Rate (see above) if it is GMP Fixed Revaluation.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Payment-Start Age` (Male and Female), `Age-Dependent Revaluation`

## Male Salary Scale

Select the Male/Female Salary Scale the salary selected

## Female Salary Scale

Select the Male/Female Salary Scale the salary selected

## Escalation Timing

Select from eitherContinuous or Review Date

## Escalation Review Date (DD/MM)

Specify a Review Date in the DD/MM format

## Payment Start Age Male

Select the Male/Female Agefor the Data field selected

## Payment Start Age Female

Select the Male/Female Agefor the Data field selected

## Age Dependent Revaluation

Select the Revaluation Rate that applies in the period up to the Age
that the numeric data field goes into Payment

## Age Dependent Increases

Select the Increase Rate that applies in the period after the Age that
the numeric data field goes into Payment

## Escalation Rate

Select the Financial Assumption that applies to the numeric data field

## Interrogate Basis

Interrogate Basis for relevant information

## Create Formula

Add a new set of adjustments

## Delete Variation

Delete a set of adjustments

## Add Variation

Add a new set of adjustments

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