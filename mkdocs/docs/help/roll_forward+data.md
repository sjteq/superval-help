# Roll Forward: Data



## Effective Date of Data File

Specify the Effective Date of the Data File by selecting from the list
of Standard Dates or specifying an alternate Date

## Roll-Forward Date

Specify the Roll Forward Date by selecting from the list of Standard
Dates or specifying an alternate Date

## Roll Forward Data File

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

## Rolled Forward CSV File

Specify a name for the data file. The filename specified must not
already exist as it will not overwrite an existing file. It will be
created in the Scheme Folder.

Double Clicking will activate the standard Windows Open File Dialog
box for selection of a file (which can be used as a `starting point` for
the name of the file).

## Financial Globals Parameter Set

Select the description of the Financial Globals Parameters

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

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