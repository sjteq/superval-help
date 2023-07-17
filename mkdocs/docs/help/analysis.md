# Analysis



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

## Analysis Data File(s)

## Analysis Data File

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

## Calculation Date

The Analysis can be carried out at any date that you wish.

## Salary Definition

The analysis or investigation of the active membership data may be based
on either the Current or Previous Salary.

## Upper Limit of Age Ranges

You must specify the age ranges to be used in the analysis. The values
specified represent the upper limits of the ranges.

The first group will include all ages less than or equal to the first
value and data beyond the last limit specified will be grouped into a
final group.

Enter the age ranges as a vector of ages, e.g. `20 30 40 60`.

## Ages Definition

Check the box to select the Method of Rounding for the Age Calculation.
The options are:

-   Age Next
-   Age Attained
-   Age Nearest

## Upper Limit of Membership Ranges

Specify the membership or service ranges to be used in the analysis. The
values specified represent the upper limits of the ranges.

The first group will include all durations less than or equal to the
first value and data beyond the last limit specified will be grouped
into a final group.

Enter the (service) duration ranges as a vector, e.g. `10 20 30 40`.

## Based on Date of Joining

The (service) duration ranges specified are calculated according to the
selection in this field and the `Calculation Date`. Check the box to
select either based on Date of joining Company or Date of joining
Scheme. The data will be taken from the standard data items,

## Salary

## Salary x Membership

## Membership

Check the box to specify how the membership data should be analysed. The
options are:

-   total and average salary for each group
-   total and average salary by service/membership for each group
-   total and average service/membership for each group.

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