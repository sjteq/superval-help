# Snapshot Salary



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

## Calculation Date

The Calculation Date to which the investigation is performed.

This defaults to the Current Valuation Date. You can overwrite this if
you wish as the investigation can be carried out at dates other than the
valuation date provided there is sufficient data.

Dates can be entered in almost any format and they will be automatically
converted to DD/MM/YYYY format.

## Start Age

The Start Age is the minimum age at which investigation results will be
output to the file (or in the review of the investigation, the graphical
display).

Note that the results for all ages are calculated (and saved). The Start
Age can be adjusted when reviewing the investigation results.

## End Age

The End Age is the maximum age at which investigation results will be
output to the file (or in the review of the investigation, the graphical
display).

It is rounded to the next highest multiple of the Grouping of Data
factor from the Start Age.

Note that the results for all ages are calculated (and saved). The End
Age can be adjusted when reviewing the investigation results.

## Grouping of Results - Every

The Grouping of Data factor determines the size of the age sub-divisions
used to summarise investigation results output to the file (or in the
review of the investigation, the graphical display).

Note that the results for all ages are calculated (and saved). The
Grouping of Data factor can be adjusted when reviewing the investigation
results.

## Salary Definition

The analysis or investigation of the active membership data may be based
on either the Current or Previous Salary.

## Investigate Only Entrants between

The cohort of members to be investigated can be controlled by specifying
two dates between which members must have joined to be included for
investigation.

A date of `01/01/1901` and the Current Valuation Date as specified
initially. This would include all members active at the Current
Valuation Date in the investigation. Dates can be entered in almost any
format and they will be automatically converted to DD/MM/YYYY format.

If your data records do not contain either of the joining dates, all
members are investigated irrespective of these parameters.

These parameters enable:

-   investigation of the promotional salary scale durationally; or
-   to investigate, for example, only members who were in-force at the
    previous valuation date.

Pairs of Snapshot Salary investigation runs can be carried out to
produce some comparable averages over the inter-valuation period.

To determine the increase in Average Scheme Salary over the
inter-valuation period (increases due to inflation only) compare the
averages from:

1.  Investigate members joining between `01/01/1901` and the Current
    Valuation Date based on Current Salary with a Calculation Date of
    the Current Valuation Date.
2.  Investigate members joining between `01/01/1901` and the Previous
    Valuation Date based on Previous Salary with a Calculation Date of
    the Previous Valuation Date.

To determine the increase in Average Salary for members in-force
throughout the inter-valuation period (increases due to inflation and
promotion) compare the averages from:

1.  Investigate members joining between `01/01/1901` and the Previous
    Valuation Date based on Current Salary with a Calculation Date of
    the Current Valuation Date.
2.  Investigate members joining between `01/01/1901` and the Previous
    Valuation Date based on Previous Salary with a Calculation Date of
    the Current Valuation Date.

## Based on Date of Joining

The (service) duration ranges specified are calculated according to the
selection in this field and the `Calculation Date`. Check the box to
select either based on Date of joining Company or Date of joining
Scheme. The data will be taken from the standard data items,

## Save the Results for Sub Groups

The results (for all files or sub-groups combined) of every
investigation are always saved (to a saved results file). These results
are stored using the description applied to the parameter set when
saved.

This option allows you to also save the results for each of the files or
sub-groups specified as well. These results are stored using the
description of the saved parameter set with a suffix of the sub-group
data filename.

Stored results for each of the sub-groups means that:

-   males and females can be investigated simultaneously but separate
    results can be reviewed; and/or
-   the appropriateness of the Rate Table found to be the best fit for
    the whole group can be checked against each of the sub-groups.

It is possible to delete stored investigation results when reviewing the
investigation. It is recommended that any results for inappropriate
groupings such as heterogeneous groups (eg males and females combined
when the decrement should clearly be different) or any small groups (for
which comparisons are not reliable) or for any runs containing erroneous
data should be deleted to avoid possible error.

## Expected Table

The Rate Table Code of the `expected` table for comparison with the
actual Scheme experience.

The starting point for the comparison table is generally the `expected`
table that was assumed at the previous investigation.

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

## Age Rating

Any Rate Table can be rated up or down by a number of years as required
to make the rate at every age `lighter` or `heavier` than in the
original table.

A value of `+10` will result, for example, in the value selected for a
30 year old actually being the rate for a 40 year old and for a value of
`-5` would mean that the value at age 25 is selected.

If an age rating of a fraction of a year is required, a new table will
have to be created through the Edit rate table option on the Rate Table
form.

## Percentage Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

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