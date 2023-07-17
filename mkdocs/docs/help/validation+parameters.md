# Validation: Parameters



## Previous Valuation Date

The Previous Valuation Date for the purposes of the validation. It is
the effective date of the Previous Salary. No warning of a blank
Previous Salary will be produced for those who joined after this date.

It defaults to the Previous Valuation Date. You can overwrite this if
you wish.

Dates can be entered in almost any format and they will be automatically
converted to DD/MM/YYYY format.

## Current Valuation Date

The Current Valuation Date for the purposes of the validation.

It defaults to the Current Valuation Date as specified on the Scheme
Details but you can overwrite this if you wish.

Dates can be entered in almost any format and they will be automatically
converted to DD/MM/YYYY format.

## Validation Data File(s)

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

## Only Records with Errors or Warnings Listed

Specify whether you want a listing for all members in the data file
(unchecked) or, alternatively, only get a listing of those members for
whom an Error or Warning has been found (checked).

## Include Warnings of Blank Numeric Fields

Specify whether you require Warnings on Numeric Fields when they are
blank.

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