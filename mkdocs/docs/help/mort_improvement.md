# Mort Improvement



## Mortality Improvement Definition

Select from the drop-down list which of the four Mortality Improvement
methods to use. The options are:

-   Calendar Year
-   Specified Year of Birth
-   Accurate Method
-   2 Dimensional Table

## Apply Mortality Rate Age Rating to Mortality Improvement Table

Check this box if the age rating being applied to the Pre Retirement,
Post Retirement and Ill Health Mortality table should also be applied to
the Mortality Improvement Factors.

For example, if a member is aged 46 nearest at valuation date and a `-2`
age rating is being applied to the Pre Retirement Mortality table. Then
if the box is unchecked, then the age that SuperVal will use at
valuation date for Mortality Improvement factors will 46. If the box is
checked, the age that SuperVal will use at valuation date for Mortality
Improvement factors will 44.

## Base Year of Mortality Table

## Base Year of Mortality Improvement Table

When using the `Specified Year of Birth`, `Accurate Member Specific` or
`2D Tables` projection methods, enter the Base Year of the Mortality
Improvement Table.

For more information please see the Infocus Document relating to
Mortality Set Up.

## Term from Base Year (Member)

## Term from Base Year (Death pre Retirement - Actives/Deferreds)

## Term from Base Year (Contingent Spouse - Actives/Deferreds/Pensioner)

This field is only required if using the Specified Year of Birth
projection method:

Enter the specified year of birth. This field would typically be set to
say, 1945.

For more information please see the Infocus Document relating to
Mortality Set Up.

## Year of Birth (Member)

## Year of Birth (Death pre Retirement - Actives/Deferreds)

## Year of Birth (Contingent Spouse - Actives/Deferreds/Pensioner)

This field is used when the Calendar Year of Birth method is selected.
Previous CMI reports have suggested a period of 20 years.

For more information please see the Infocus Document relating to
Mortality Set Up.

## Alpha Factor - Ultimate Improvement

If either of the `Calendar Year`, `Specified Year of Birth` or `Accurate
(Member Specific)` Methods has been selected then double click to select
the age related rate table (e.g. type `HX`) containing the values for
alpha(x) at each age.

CMI No. 10 suggests alpha(x) to be as follows:

\= 0.5 for age &times;&lt;60

\= 0.01(x-10) for age 60 &times; 110

\= 1 for age &times;&gt;110

CMI No. 17 suggests alpha(x) to be as follows:

\= 0.13 for age &times;&lt;60

\= 1+0.87(x-110)/50 for age 60 &times; 110

\= 1 for age &times;&gt;110

For more information please see the Infocus Document relating to
Mortality Set Up.

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

## Beta Factor - % of Mortality Improvement

## Attained after Period of Years

If either of the `Calendar Year`, `Specified Year of Birth` or `Accurate
(Member Specific)` Methods has been selected then double click to select
the age related rate table (e.g. type `HX`) containing the values for
beta(x) at each age.

CMI No. 17 suggests an age related step function after 20 years
(suggested beta(x) for f20). SuperVal requires a `HX` type table
containing the beta(x) values:

Beta(x)

\= 0.55 X&lt;60

\= 0.55 &times; (110-X)/50 + 0.29 &times; (X-60)/50 60≤X≤110

\= 0.29 X&gt;110

CMI No. 10 suggests a value of 60% after 20 years (suggested value for
f20); SuperVal requires an `HX` type table containing 0.6 for all ages.

For more information please see the Infocus Document relating to
Mortality Set Up.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Two-Dimensional  Improvement Table (CSV File)

If `2D Tables` has been selected or you are entering the PPF Overrides,
the select from the drop-down list which of the available tables to use.
The user will be able to select from the CSV files stored in the Library
Folder containing the mortality improvement rates.

Version 9 is supplied with a sample 2D file called `MortImpNew.csv`.

The CSV file should contain 120 rows and 120 columns. Ages are held in
the rows and Years in the Columns. The table should start at age 0 and
the Year that your Table starts. If no year is entered SuperVal will
assume this starts at Year 2000.

## Two-Dimensional  Improvement Table (Rate Table)

If `2D Tables` has been
selected, then users can upload mortality improvement tables into the
`SVDECR.SF` file.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

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