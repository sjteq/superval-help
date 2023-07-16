# Contributions



## Contributions Method

Select from the drop-down list which of the 5 contribution methods to
use. The options are:

-   Fixed Percentage of Salary
-   Differing Percentage on up to 10 Salary Bands
-   Varying Percentage of Salary based on Attained Age
-   Varying Percentage of Salary based on Age at Entry
-   Salary Bands Table with Differing Percentages

Not all functionality is available to all users.

## Contribution Rate

If `Fixed Percentage of Salary` has been selected, enter the Fixed Rate
Contribution as a percentage i.e. for 5% enter `5` rather than `0.05`.

## Lower Band Amount

If `Differing Percentage on up to 10 Salary Bands` has been selected,
then enter the salary amount from which the adjoining contribution rate
will be paid on i.e. the salary the contribution band starts from.

To add a new row, right click over a number in the first column. You
will then be able to select how many rows to add, whether to insert a
new row or delete a row.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Contribution Rate %

If using `Differing Percentages on up to 10 Salary Bands`, then enter
the Contribution Rate that applies on earnings between the Salary Band
Limit to the left of this field and the Salary Band Limit below.

If using `Salary Bands Table with Differing Percentages`, then enter the
Contribution Rate that applies to the salary bands.

### Related



-   [Adding and deleting rows](adding_deleting_rows.md)

-   [Grid editing options](grid_editing_options.md)

## Grid Help

Right-clicking on a column heading presents a menu with the following
options which allow you to expand or reduce the number of columns of
data to be entered:

-   Add a new column to the right of the grid;
-   Insert a new column at the position of the cursor; and
-   Delete the current column at the position of the cursor.

## Grid Help

Right-clicking on the Top Left Corner of the grid displays a menu which
allows you to set the following Grid Editing Options:

-   Editing of a cell can be invoked by either clicking on the cell or
    by pressing F2 when the cell is active (Clicking will only change
    the current active cell); and
-   determine the cursor movement once editing is complete to be either
    to the next cell down, the next cell to the right or to stay in the
    current cell.

## Contributions Band Method

If `Differing Percentage on up to 10 Salary Bands` or `Salary Bands
Table with Differing Percentages` has been selected, then select from
the drop-down list the method for determining how the contribution rates
are applied to the Salary Bands. The options are:

-   Progressive
-   Band-Related

If `Progressive` is selected, then the different contribution rates
apply to each band of earnings, in a similar way to income tax. For
example, say we have the bands below. The contributions paid for a
member earning £100,000 are set out in the table below.

Band | Range           | Employer Contribution Rate | Contributions Calculated As
-----|----------------:|---------------------------:|----------------------------
1    | 0 – 12,600      | 5.5%                       | 0.055 &times; £12,600 = £693 on her Band 1 earnings
2    | 12,601 – 14,700 | 5.8%                       | 0.058 &times; £(14,700–12,600) = £121.80 on her Band 2 earnings
3    | 14,701 – 18,900 | 5.9%                       | 0.059 &times; £(18,900–14,700) = £247.80 on her Band 3 earnings
4    | 18,901 – 31,500 | 6.5%                       | 0.065 &times; £(31,500–18,900) = £819.00 on her Band 4 earnings
5    | 31,501 – 42,000 | 6.8%                       | 0.068 &times; £(42,000–31,500) = £714.00 on her Band 5 earnings
6    | 42,001 – 78,700 | 7.5%                       | 0.075 &times; £(78,700–42,000) = £2,752.50 on her Band 6 earnings
7    | 78,701 – 81,500 | 7.7%                       | 0.077 &times; £(81,500–78,700) = £215.60 on her Band 7 earnings
8    | 81,501 – 84,000 | 7.9%                       | 0.079 &times; £(84,000–81,500) = £197.50 on her Band 8 earnings
9    | 84,001 – 89,000 | 8.2%                       | 0.082 &times; £(89,000–84,000) = £410.00 on her Band 9 earnings
10   | &gt;89,001      | 8.5%                       | 0.085 &times; £(100,000–89,000) = £935.00 on her Band 10 earnings
     |                 |                            | Total Contributions Paid would be £7,106.20 per year

If `Band-Related` is selected then a single contribution rate is paid
based on the member’s total salary. The rate depends on the Band in
which the member’s salary lies. Under this approach, the contributions
paid for a member earning £100,000 would be calculated as 0.085 &times;
£100,000 = £8,500 per year. (The member’s salary lies in the range
covered by Band 10 and so the Band 10 contribution rate is applies to
their entire salary.)

## Earnings Bands Increase

If `Differing Percentage on up to 10 Salary Bands` has been selected,
this is the rate at which the [Salary Band
Limits](#contributions+gcdband) on which the contributions are based
will be increased in the future.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable.

Once selected, the current value of the Global Financial Parameter is
shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this yab.

## Contribution Rate Salary Bands Table

Enter the Salary Band Limits that apply on the anniversary of the
valuation date in the [Base Year of Salary Band
Table](#contributions+gcdsalbase).

The entries in Band 0 correspond to the bottom of the first salary band
ie the salary level at which contributions start.

The number of entries for each band does not need to be identical.
However, the geometric mean of the last two values will be used for all
years into the future. (To use a particular value into the future ensure
this is entered into the last two durations.)

The contribution salary at the mid-point will be compared with the
geometric average of the Salary Band Limit at the beginning and end of
year.

The maximum number of Salary Band Limits is 10. (This is consistent with
9 salary bands.)

Not all functionality is available to all users.

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

## Base Year of Salary Bands Table

If `Salary Bands Table with Differing Percentages` has been selected
then enter the Base Year for the table of salary bands. (This will
enable the same Table to be used in a subsequent valuation year if the
bands and increases are unchanged.)

Not all functionality is available to all users.

## Contribution Rate Age Table

If `Varying Percentage of Salary based on Attained Age` or ` Varying
Percentage of Salary based on Age at Entry` has been selected, the
double click to select the Rate Table containing the contribution rates
for each age or age at entry. A typical rate table would be of type `FX`
(but `EX`, `GX`, or `HX` could all be used).

The values in the table should be entered as percentages i.e. for 5% the
entry should be `5` and not `0.05`.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Contribution Rate Duration Table

Specify the Table Code of the Contribution Rates

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Based on

If `Varying Percentage of Salary based on Age at Entry` has been
selected, then select from the drop-down list how age at entry should be
determined. The options are:

-   Scheme Membership
-   Company Service

If Scheme Membership is selected the age at entry will be determined
from the standard data item DJF (Date Joined for Pensionable Service).
If Company Service is selected the age at entry will be determined from
the standard data item DJS (Date Joined for Company Service).

## Contributions Cease after

If contributions cease after a number of years service, enter the
maximum number of years here. If no maximum period of service exists
then enter `99` here.

## Based on

The field is used to determine how the maximum service for contributions
is calculated. Select from the drop-down list from:

-   Scheme Membership
-   Company Service

If Scheme Membership is selected the maximum number of years
contribution will be determined from the standard data item DJF (Date
Joined for Pensionable Service). If Company Service is selected the
maximum number of years contribution will be determined from the
standard data item DJS (Date Joined for Company Service).

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

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