# Constants



## Variable Name

Scheme Constants can be used to define loading factors that change with
the financial basis for the scheme.

Enter a name for the Global Financial Parameter or the Constant being
defined.

This name will be used to select the Global Financial Parameter in the
individual basis files. The name should be generic i.e. InterestRate1 so
that it remains relevant if the value changes at a future valuation
date. The purpose of these variables is to enable a simple method of
making changes to assumptions without the need to modify all category
sets.

The Variable Name must not be the same as a Variable Name already used
in SuperVal system. Using an existing Variable Name may cause a system
crash or result in incorrect results for the calculations.

To add or delete a Global Financial Parameter right click over the
numbers to the side of this table. To change a Global Variable Name
click once over the existing name until the name is highlighted.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Variable Value

Enter the Global value for the variable or constant.

The rate can be input as either a single rate, a vector or a yield
curve.

For a single rate, enter the value. For 6% enter `6` and not `0.06`.

For a vector, enter the appropriate rates i.e. if 3 4 5 was entered then
the rate of increase would be 3%, 4% and 5% in the first and second year
after the valuation date and 5% thereafter.

For a yield curve, right click to choose the CSV file containing the
relevant data. The CSV file should contain one row with a maximum of 200
numbers i.e. 200 columns. The CSV file should be saved in the input
folder.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Comment

Enter a description for the Global Financial Parameter i.e. Interest Rate
for ex ABC Staff or the Constant being defined. Where possible the
description should be generic so that it remains relevant if the
absolute value of the variable changes at a future valuation date.

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