# Rate Tables



## DECRFile

The top node has the name of the Decrement File that is being displayed.
This is the Decrement File for the Scheme that is contained in the
Scheme Details.

Each type of Rate Tables has a parent node with a description of the
Rate Tables. Rate Tables are displayed in the following order:

-   Decrement Rates
-   Salary Scales
-   Durational Weights
-   Proportion Married
-   New Entrant Tables
-   Annuity Tables
-   Miscellaneous tables.

Within each type Rate Tables are ordered by the Rate Table number.

Once an individual rate table has been selected, a graph of the rate
table is shown on the upper right section of the screen. Double clicking
on the graph will expand this. Once expanded, you can right-click to
obtain additional functionality i.e. printing.

See the Infocus document called Using Rate Tables for more information
on this area of SuperVal.

## Table Code

The Table Number field is a display only field showing the Rate Table
Code used to identify the Rate Table.

With effect from V9.03, SuperVal Rate Tables can be prefixed by both an
upper case and a lower case letter. (Previously all Rate Tables had an
upper case letter.) This acts to double the number of Rate Tables
available but care must be taken to ensure the intended table is
selected.

## Table Description

The description of the Rate Table for identification purposes.

## Age

## Rate

## Duration

At the bottom of the screen, the values in the Rate Table are displayed
in the &lsquo;spreadsheet&rsquo;.

The range of Rates that can be specified are:

-   ages 0 to 119 for Age related Rate Tables (including Miscellaneous
    X-tables)
-   durations 0 to 59 for Duration related Rate Tables (including
    Miscellaneous T-tables)
-   dimensions (related to Age (Y-axis) and Duration (X-axis) for
    decrement rates) of 120 values for 2-Dimensional Rate Tables
    (including Miscellaneous M tables).

The format of the Rates being entered will depend on the type of Rate
Table being entered.

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

## Select

When the Rate Tables form has been called by double-clicking on a Rate
Table field, a _Select_ button will become available.

On pressing the _Select_ button, the Rate Table form will be closed down
and the currently highlighted Rate Table will become the value of the
Rate Table field.

A Rate Table can also be selected by double-clicking on its node.

## Edit

When a Rate Table is highlighted (and you have been given the
appropriate access level), an Edit Button will become enabled.

On pressing the _Edit_ button, the Rate Table (and its Rate Table number
and description) can be modified.

Note that after the _Edit_ button is pressed and until the editing is
completed or aborted, the Rate Table file is locked to stop other users
from making simultaneous changes to this Rate Table file (which may
cause corruption of the file). Thus it is recommended that the shortest
time possible be spent in this mode.

## Add

When a parent node of a group of Rate Tables is highlighted (and you
have been given the appropriate access level), an _Add_ button will become
enabled. This will also be used to add another Factor Table.

On pressing the _Add_ button, the Rate Table number, description and rates
can be specified.

Note that after the _Add_ button is pressed and until the addition is
completed or aborted, the Rate Table file is locked to stop other users
from making simultaneous changes to this Rate Table file (which may
cause corruption of the file). Thus it is recommended that the shortest
time possible be spent in this mode.

## Delete

When a Rate Table or Factor Table is highlighted (and you have been
given the appropriate access level), a Delete Button will become
enabled.

On pressing the _Delete_ button, the Rate Table/Factor Table will, after
confirmation, be deleted.

Note that after the _Delete_ button is pressed and until the deletion is
completed or aborted, the Rate Table file is locked to stop other users
from making simultaneous changes to this Rate Table file (which may
cause corruption of the file). Thus it is recommended that the shortest
time possible be spent in this mode.

## Print

Pressing the _Print_ button enables the printing of Rate Tables. The Rate
Tables printed will depend on the node that is highlighted when the
Print button is pressed as follows:

-   If the top node (with the Rate Table filename) is highlighted, a
printout of all Rate Tables on that Rate Table file will be
prepared.
-   If Rate Table type description is highlighted, a printout of all
Rate Tables of that type on that Rate Table file will be prepared.
-   If an individual Rate Table is highlighted, a printout of that
particular Rate Table will be prepared.

## Export

Click the _Export_ button to export the rate table into Excel as either a
CSV file or a XLS file. The exported file will be found in the Library
folder of SuperVal.

For more information on Exporting Rate Tables, see the Infocus document
called Using Rate Tables.

## View

Pressing the _View_ button enables the display of a 2-Dimensional Rate
Tables in a larger frame.

## Quit

Clicking on the _Quit_ button allows you to exit without saving any of
your changes.

In some of the screens you will be asked to confirm if you want to exit
_Ignoring all changes_. If you click _Yes_, the file will be closed
without saving any changes. If you click _No_ you will be returned to your
original screen.

From the Browser, the _Quit_ button will take you to a graphical display
of the results.