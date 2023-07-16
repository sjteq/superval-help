# Approximate GMP



## Calculation Date

The Calculation Date to which the calculation is performed.

This defaults to the Current Valuation Date. You can overwrite this if
you wish as the calculation can be carried out at dates other than the
valuation date provided there is sufficient data.

Dates can be entered in almost any format and they will be automatically
converted to DD/MM/YYYY format.

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

## Salary

Select from the drop-down list which of the salaries defined on the
Salary Tab to use in the calculation of the approximate GMP.

## Lower Earnings Limit

Select from the drop-down list the Lower Earnings Limit applying at the
calculation date.

## Upper Earnings Limit

Select from the drop-down list the Upper Earnings Limit applying at the
calculation date.

## Minimum Start Date

Enter the Minimum Start Date for the calculation of the accrued GMPs.

## Maximum End Date

Enter the Maximum End Date for the calculation of the accrued GMPs.

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