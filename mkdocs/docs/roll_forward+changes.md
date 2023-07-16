# Roll Forward: Changes



## New Members Data File

Double click to select the filename (or filenames, if appropriate) of
the member data files to be processed.

Data files may contain inactive members (exits and members who have
joined after the valuation date) as well as active members.

The file(s) must be in the format specified in the data format.

If specification of only one file is allowed, a list of the allowable
files specified on the Scheme Details will be presented with a Right
Click. Note that any filenames used on that list will be `relative
value`, that is, the filename specified is controlled by the label to
the right of the field. If the filename is changed on the Scheme Details
then the filename in the saved parameters will also be change.

## New Members Data Format

Double click to select the Format File for the current Data File. The
Format File contains the saved parameters specifying the column
specification of each of the data items contained in the data file. Data
format descriptions are prefixed by an indication of the type of format
e.g. &lt;Act&gt; for Actives, &lt;Def&gt; for Deferreds, &lt;Pen&gt; for Pensioners.

If you intend to use the GMP Calculators to calculate GMPs after
creating your data, ensure that columns are created in your data file
for these fields. (In addition, enter dummy data into the data file for
the first member that is at least as large as the largest expected GMP
for all members. This will ensure that the Format created leaves
sufficient space for the GMPs calculated.)

## Data&gt;Build

If you have created data using _Data&gt;Build_ then the format name will
be the same as the original source (CSV) file.

## BasisModule&gt;Migrate

If you have migrated your data files from earlier versions the name will
be unchanged.

## Exit Identifier 1

Select a data field to be used to identify members who have exited

## Exit Identifier 2

Select a second data field to identify members who have exited.
Selecting a second Identifier will display an additional column in the
Exited Members grid

## Calculate Estimated Benefit as Liability for Exited Members

Indicate if a liability for Exited Members is to be calculated based on
an Estimated benefit

## Identifier1

Enter the Name of the Member who has exited the Scheme

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Identifier 2

Enter the second identifier value for the member who has exited the
Scheme

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Date Of Exit

Define the Excited Member’s Date of Exit

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Mode Of Exit (Estimated Liability)

Select a Mode of Exit

mode       | Actives | Deferreds | Pensioners
-----------|:-------:|:---------:|:---------:
Withdrawal | X       |
Ill-health | X       |
Retirement | x       | x
Death      | x       | x         | x

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