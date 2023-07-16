# ActFormat: Non Standard

The following page shows the Data Format for the Non-Standard Data
Items.

These are broken down into "Total" Numerical Fields, "Average" Numerical
Fields, Character Fields and Date Fields.

Please note that when creating your data, any Non-Standard data items
will have included in the header row details of whether it is a
Character Field, a Numeric Field or a Date Field.  The Numeric Fields
can either be Totals or Averages and are distinguished by a capital "N"
for a total and a lower case "n" for an average field.  The user should
ensure that any salary, pension and accumulated contributions are shown
under the "Total" Numerical Fields and that any service fields, such as
added years, are shown under the "Average" Numerical Fields.


## Variable Name

This column will show the non-standard Variable Name loaded from the
data file. Where possible, the user should use a descriptive name for
the variable to enable easier identification at a later stage. All
non-standard Variables should be prefixed with a q.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Current From

## Current To

## From

## To

## Date Format

For each of the non-standard data fields, this will show the start and
end columns of where the data item is located in the data file.

For date fields, specify the date format e.g. DD/MM/CCYY. The year
portion must have 4 digits.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Previous From

## Previous To

If Analysis of Surplus calculations are required it is necessary, for
each of the numeric non-standard data fields, to specify the start and
end columns of where the data item applicable at the previous valuation
date is located in the data file.

If the value of a numeric field has not changed over the inter-valuation
period, the same columns (exactly) can be specified for both the current
and previous data items.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Description

It is possible to give each non-standard data field an optional
description for easier identification.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

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

## Migrate

Pressing the _Import_ button pops up a window which allows you to import a
Superval/21 data format.

## Display

Using the _Display_ button while looking at Rate Tables will display the
changes made to the currently specified rate table.  
Pressing the _Display_ button elsewhere pop-ups a window which allows you
to display a member record with a ruler to determine column
specifications. On the Display window, you can specify the name of the
data file (.dat file) and record number from that file.

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