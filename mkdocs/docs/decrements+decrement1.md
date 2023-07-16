# Decrements: Decrement1



## Exit Description

A description of the type of decrement to be investigated.

A different description for each of the types of decrement will enable
identification when browsing the output and displaying the results.

## Modes of Exit to be Analysed

Select one or more Modes of Exit to be investigated from the list.

Any number of modes of exit can be specified to be investigated in
combination to represent one cause of exit (for example when you are
investigating all forms of age retirement – normal, early and late).

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

## Upper Limit of Durations Analysed

Specify the Upper Limits of the Durations to be investigated (subject to
the limit that only 20 years of durational experience is stored).

To enable you to build durational specific rates of withdrawal, the
exposure and actual exits for all decrement investigation runs are
calculated by both age and duration (up to 20 years, beyond that is
grouped into an &ldquo;ultimate&rdquo; group).

You can specify a series of upper limits of Durations to be Analysed in
which decrements will be investigated. The lower limit will be one
greater than the previous upper limit specified. If, say, the first
upper limit specified is `5`, rates will be calculated in respect of
exits and exposure contributed in the first five years of Scheme
membership.

If ultimate rates only are required, specify an upper limit greater than
20, eg the default of `99` suggested.

A separate page of output will be produced for the durations between
each pair of durations specified.

Note that the exposure and number of exits is saved for all durations up
to 20 years so the upper limits on the Durational Ranges can be
subsequently changed when producing the graphical displays.

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

## Durational Weight Table

In connection with the ability to calculate Durational Specific rates of
withdrawal, if the `Expected Exits` Table Type is a Withdrawal (or
Leaving Service) Table, a Withdrawal Durational Weight Table may be
applied to the standard table.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

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