# File Calculator



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

## Output Data File

Specify a name for the data file. The filename specified must not
already exist as it will not overwrite an existing file. It will be
created in the Scheme Folder.

Double Clicking will activate the standard Windows Open File Dialog
box for selection of a file (which can be used as a `starting point` for
the name of the file).

## Input Field 1 - Numeric (FV1)

## Input Field 2 - Numeric (FV2)

## Input Field 3 - Numeric (FV3)

You can specify up to three numeric data fields to be used in the
calculation of the new numeric or date input data field.

For each of these numeric input data fields, it is necessary to specify
the start and end columns of where the numeric data item is located in
the input data file.

A Right Click allows you to select a numeric data field defined in the
data format specified.

## Input Field 4 - Character (FV4)

You can specify one character data field to be used in the calculation
of the new numeric or date input data field.

For this character input data field, it is necessary to specify the
start and end columns of where the character data item is located in the
input data file.

A Right Click allows you to select a character data field defined in the
data format specified.

## Input Field 5 - Date (FV5)

## Format

## Input Field 6 - Date (FV6)

You can specify up to two date data fields to be used in the calculation of the new numeric or date input data field.

For each of these date input data fields, it is necessary to specify the start and end columns of where the date data item is located in the input data file.

Date fields may be in any format which must be specified as a combination of 2 or 4 `Y`s, 2 `M`s and 2 `D`s with either `-` or `/` as a delimiter.

A right click allows you to select a date data field defined in the data format specified.

## Formula for New Data Field

The formula to calculate the value of the calculated input data field is
specified in APL Coding. The values contained in the data fields should
be specified as:

-   FV1, FV2 and FV3 for the three numeric input data fields
    respectively;
-   FV4 for the character input data field; and
-   FV5 and FV6 for the two input date fields respectively.

In addition to the functions that can be used in coding of benefits, the
following functions are also available:

`date1 DATEMAX date2` 

: the result is the later of the two dates specified (either of which may be fixed date expressed in DD MM YYYY)

`date1 DATEMIN date2`

: the result is the earlier of the two dates specified 
	(either of which may be fixed date expressed in DD MM YYYY)

`days DATEOFFSET date` 

: the result is the date offset by the number of days.

This formula is checked (as far as possible) for syntax etc. before the
run is executed.

## Output Field

## to

You must specify the start and end columns (both inclusive) of the
output data field where the calculated result is to be inserted in the
data records.

This field can overwrite an existing data field in the records
(including one of the input data fields from which the result is being
calculated).

If necessary, the output data field may be beyond the end of the member
record and the member data records will be lengthened to accommodate the
field (including moving the last column which fixes the length of the
records). Note that it will be necessary to modify the data format if
this is done.

Ensure you specify sufficient columns to fit the largest possible result
(including the decimal point, if any) as an error will be reported if
all results do not fit.

## Decimal Places

If the calculated result is numeric, the number of decimal places to be
displayed in the calculated data field must be specified. Note that this
must be at least two positions less than the length of the output data
field.

## OR Date Format

If the calculated result is a date, the format of the date must be
specified. The format of the date can be different from the format of
the input date(s).

The date format can be a combination of 2 or 4 `Y`s, 2 `M`s and two `D`s with
either `-` or `/` as a delimiter.

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