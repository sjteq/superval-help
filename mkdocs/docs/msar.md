# MSAR



## Input Data File

Specify the input data file (or files, if appropriate). It must be
located in the Scheme Folder.

Double Clicking will activate the standard Windows Open File Dialog
box for selection of a file.

## Data Format

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

## Accrual Start Date

Specify a fixed date in DD/MM/CCYY format for start date of the period
of accrual. If the start date is a member data item then select this
from the drop-down list.

## Accrual Finish Date

Specify a fixed date in DD/MM/CCYY format for the finish date of the
period of accrual. If the finish date is a member data item or `DOBADD`
select this from the drop-down list.

## Service Calculation - Period

## Rounding

Select from the drop-down list what service rounding to apply in the
calculations. The options are:

-   Days
-   Months
-   Years

## Male Normal Retirement Age

## Female Normal Retirement Age

Specify the Normal Retirement Age i.e. the age at which it is should be
assumed the member will retire.

## Total Accrual

Enter the target percentage accrual that the members should receive at
the end of the period. The period is defined by the start and finish
dates. The target percentage can either be a fixed rate (for all members
in the data file) or a member data item.

To enter a fixed percentage, enter the percentage here i.e. for a target
2/3rds accrual enter `66.667` rather than `0.66667`.

To enter a member data item, the select from the drop-down list the data
item containing the relevant percentage.

To enter an Accrual Rate Table, ensure this field is left blank.

## Accrual Rate Table

Enter the code for the cumulative accrual rate table (type `HT`).
Members will achieve the pension percentage at the end of the period
between start and finish dates shown in the table.

Please note that only one of the accrual rate fields can be used i.e.
one of:

-   Accrual Percentage (fixed)
-   Accrual Percentage (data item)
-   Accrual Rate Table

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

## Minimum Numerator

The accrual rate data item that is calculated can be subject to a
minimum and a maximum. Enter the numerator of any minimum accrual rate
required in this field.

For example to satisfy the Reference Scheme Test you may wish to set a
minimum of 1/80ths. If this is the case enter `1` in this field.

Enter zero in this field to ignore any minimum accrual rate.

## Denominator

The accrual rate data item that is calculated can be subject to a
minimum and a maximum. Enter the denominator of any minimum accrual rate
required in this field.

For example to satisfy the Reference Scheme Test you may wish to set a
minimum of 1/80ths. If this is the case enter `80` in this field.

Enter zero in this field to ignore any minimum accrual rate.

## Maximum Numerator

The accrual rate data item that is calculated can be subject to a
minimum and a maximum. Enter the numerator of any maximum accrual rate
required in this field.

For example to satisfy Inland Revenue Maximum you may wish to set a
maximum of 1/30ths. If this is the case enter `1` in this field.

Enter zero in this field to ignore any maximum accrual rate.

## Denominator

The accrual rate data item that is calculated can be subject to a
minimum and a maximum. Enter the denominator of any maximum accrual rate
required in this field.

For example to satisfy Inland Revenue Maximum you may wish to set a
maximum of 1/30ths. If this is the case enter `30` in this field.

Enter zero in this field to ignore any maximum accrual rate.

## Output Data File

Specify a name for the data file. The filename specified must not
already exist as it will not overwrite an existing file. It will be
created in the Scheme Folder.

Double Clicking will activate the standard Windows Open File Dialog
box for selection of a file (which can be used as a `starting point` for
the name of the file).

## Decimal Places in Accrual Rate

Enter the number of decimal places you would like the accrual rate
calculated to.

## Display

Using the _Display_ button while looking at Rate Tables will display the
changes made to the currently specified rate table.  
Pressing the _Display_ button elsewhere pop-ups a window which allows you
to display a member record with a ruler to determine column
specifications. On the Display window, you can specify the name of the
data file (.dat file) and record number from that file.

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