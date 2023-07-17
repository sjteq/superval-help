# Decrements: General



## Automatic Sex/Category Sub-File Creation

The sub-groups of membership data to be processed can be specified in
one of two ways:

If the Automatic Sex/Category Sub-File Creation box is unchecked, the
user will be asked to specify a list of data files (which have been
previously created) containing the data for each of the sub-groups
separately.

If the Automatic Sex/Category Sub-File Creation box is checked, the user
will specify a single file (containing the data for all groups) and then
select the sex and category combinations that you wish to be processed
(sex/category sub-files will be automatically created).

## Investigation Data File(s)

## Investigation Data File

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

## Select by Sex

If the _Select by Sex_ box is unchecked, the user will not see the sex listed
in the Sex/Category selection below. The list will only show list of
categories

If the _Select by Category_ box is checked, the user will the sex listed in
the Sex/Category selection below.

## Select by Category

If the _Select by Category_ box is unchecked, the user will not see the
categories listed in the Sex/Category selection below. The list will
only show Males and Females.

If the _Select by Category_ box is checked, the user willsee the categories
listed in the Sex/Category selection below.

## Sex/Category Selections

Specify the category data you wish to use.

User may also select a blank category if they do not wish to run that
particular category.

## Start Date

Enter the Start Date from which the analysis or investigation is
performed.

This defaults to the Previous Valuation Date. You can overwrite this if
you wish as any analysis or investigation can be carried out for periods
other than the inter-valuation period provided there is sufficient data.

Dates can be entered in almost any format and they will be automatically
converted to DD/MM/YYYY format.

## End Date

Enter the End Date on which the analysis or investigation is performed.

This defaults to the Current Valuation Date. You can overwrite this if
you wish as any analysis or investigation can be carried out for periods
other than the inter-valuation period provided there is sufficient data.

Dates can be entered in almost any format and they will be automatically
converted to DD/MM/YYYY format.

## Based on Date of Joining

The (service) duration ranges specified are calculated according to the
selection in this field and the `Calculation Date`. Check the box to
select either based on Date of joining Company or Date of joining
Scheme. The data will be taken from the standard data items,

## Exposure Weighting

The exposure calculated can be weighted using one of the following
options:

-   Number Weighted
-   Greater of Salaries
-   Current Salary Weighted
-   Previous Salary Weighted

## DecSelect1

## DecName1

## DecSelect2

## DecName2

## DecSelect3

## DecName3

## DecSelect4

## DecName4

## DecSelect5

## DecName5

## DecSelect6

## DecName6

## DecSelect7

## DecName7

## DecSelect8

## DecName8

## DecSelect9

## DecName9

Up to 9 different decrements can be investigated simultaneously
(although not all need be mutually exclusive, for example, one could
investigate withdrawal due to all causes including retirement and
retrenchment and voluntary withdrawal only in different decrements).

Results will be separately produced for each of the different decrements
investigated (eg Retirement, Death and Withdrawal).

For each decrement to be investigated, it necessary to check a box
(relating to the other 9 tabs on the form) and specify the name of the
decrement i.e. Withdrawal, Death. This name will then be used as the name
of the tab for identification. The user will then be required to enter
the settings for the Individual Decrements on the relevant tab.

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