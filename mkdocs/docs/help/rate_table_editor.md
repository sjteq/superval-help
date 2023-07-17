# Rate Table Editor



## Table Code

The Table Number field contains a list of available Rate Table Codes.

In Add mode, the list will contain all unused Rate Table codes (of the
particular type being added) for selection of the new Rate Table code.

In Edit mode, the list will contain the Rate Table code being edited
plus all unused Rate Table codes (of the particular type being added)
for selection of the Rate Table code. By selecting a new Rate Table
code, a new Rate Table can be created based on the values of an existing
Rate Table (or the existing Rate Table can be renamed).

## Table Description

The description of the Rate Table for identification purposes. This
description can be modified as required.

## Edit 1D Rate Tables in a Column format

Select this field to edit 1 dimensional rate tables in a column format.
This makes copying and pasting of rates quicker.

## Replace Original Rate Table with New Rate Table

When in Edit mode and if a new Rate Table code is selected, you should
indicate if the existing Rate Table is to be replaced by the new Rate
Table.

This enables you to either:

-   create a new Rate Table based on the values of an existing Rate
    Table (and not replace the existing Rate Table); or
-   rename an existing Rate Table (by replacing the existing Rate
    Table).

## Age

## Rate

## Duration

The values in the Rate Table are displayed and can be modified in the
`spreadsheet`.

The range of Rates that can be specified are:

-   pages 0 to 119 for Age-related Rate Tables (including Miscellaneous
X-tables)

-   durations 0 to 59 for Duration related Rate Tables (including
Miscellaneous T-tables);

-   dimensions of up to 120 values (related to Age (Y-axis) and Duration
(X-axis) for decrement rates) for 2-Dimensional Rate Tables (including
Miscellaneous M tables); and

-   ages 0 to 119 and durations 0 to {select period +1} for Select Rate
Tables. The mortality suffered by an individual member follows a
diagonal of the table so the Rates entered at each age (i.e. a row) for a
$t$-year select period are 

        q[x]:0, q[x-1]:1, q[x-2]:2, ..., q[x-t+1]:t-1, qx{Ultimate}

Only one column of Ultimate rates should
be specified as all durations beyond `t` year select period will use the
Ultimate rates column.

The format of the Rates being entered will depend on the type of Rate
Table being entered (an `out of range` error will be reported if an
invalid entry is input). It is necessary to input decimal points.

## Duration-related 2D tables

To determine the age used to look up the factor in Duration-Related
Decrement Tables, SuperVal will calculate both the Age Exact and the
Age Nearest at the start of the year. If Age Exact is less than Age
nearest, SuperVal will use the Age Nearest to look up the decrement at
point of exit. If Age Exact is greater than (or equal) to Age Nearest,
SuperVal will use the Age Nearest + 1 to look up the decrement at point
of exit.

To determine the service used to look up the decrement, SuperVal will
calculate the period from Date of Entry into Qualifying Service/Start
Date for Augmentation Table and anniversary of valuation date +1.

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

## De-Interpolate Rates

(2) Use this functionality to create Exact-Age rates (y) from mid-Year
rates (x).

Exact-Age rates are calculated as follows:


$$y(NRA) = x(NRA)$$

$$y(NRA-1) = 2x(NRA) - y(NRA)$$

$$y(NRA-2) = 2x(NRA-1) - y(NRA-1)$$

...

## Insert Annuities

Click the _Insert Annuities_ button to enable the calculation of annuity
factors. These values will replace values at the ages specified in the
annuity calculation.

## Delete Rates

When Adding or Editing an Age or Duration related Rate Table, pressing
the _Delete Rates_ button enables the deletion of rates in a specified
range.

## Insert Rates

When Adding or Editing Age or duration related Rate Tables, pressing the
_Insert Rates_ button enables the insertion (or replacement) of rates in a
range using a vector.

## Import Rates (Scheme)

Pressing the _Import Rates_ button enables importing rates from an ASCII
file.

The standard Windows dialog box is presented allowing you to select a
file containing the rates to be imported.

The file can be either a Text file or CSV (Comma Separated Values) file
and should contain

-   for Age and Duration related Rate Tables, a series of numbers being
alternate values of Age/Duration followed by a Rate (similar to the
`.TAB` export files created by SuperVal)
-   for 2-Dimensional Tables, a series of records containing Rates for
each respective Age (or Y-axis dimension).

It is not necessary to specify a rate for every Age and/or Duration in
the file as the default value will be assumed (one for Duration
related tables and zero for all other tables) for any unspecified
Ages/Durations.

However, the file is assumed to contain Rates for all Ages and/or
Durations so all existing rates in the Rate Table are replaced by the
imported rates.

After accepting the parameters, the effect of the import is displayed
for confirmation before the Rate Table is updated.

More information can be found in the Infocus document relating to
Importing of Rate Tables.

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