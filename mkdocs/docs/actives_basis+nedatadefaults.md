# Actives Basis: NEDataDefaults



## Male New Entrant Salaries Table

## Female New Entrant Salaries Table

Double click to select the table containing annual salary data for New
Entrants. This is an `NS` type table which contains the New Entrant
Salaries at each age.

Note that the New Entrant Salary Rate Table is assumed to be an annual
salary for a new entrant and therefore could be different to the
frequency specified in the data format.

The level of salary entered will be relevant where there are fixed
deductions, maximums or minimums to the benefits i.e. Basic State Pension,
LEL or Earnings Cap.

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

## % Rating

A percentage adjustment can be made to either a Rate Table or a Salary.

The Rate Tables can be adjusted by a percentage loading to make the
decrement rate lighter or heavier than the original table. The salary
for new entrants can be loaded to reflect changes in the salary profile.

Enter the number as percentage above 100% i.e. if a loading of 110% is
required then enter `10` or if a loading of 90% then enter `-10`. If no
adjustment is required then leave blank.

## Value

Specify the value of the Numeric Data Default that should be used for
the new entrants in the New Entrants Runs.

The user should specify the absolute value and the number of decimal
places to use.

If you wish to consider a member specific value for each member then
contact a member of the SuperVal support team for more information.

## Decimal Places

In order to get the correct precision, you must specify the number of
decimal places to be displayed.

An input data field such as a Benefit Multiple will require a few
decimal places but an accumulation of contributions will be accurate
enough if rounded to the nearest pound. The Data File created will
contain the values entered into the Value field rounded to this number
of decimal places.

## Type

The type field is a display only field reminding you of the type of the
numeric data item.

The distinction is only relevant for the New Entrant Model Replacement
when multiple members are assumed in the New Entrant Proportions. The
New Entrant Data Default for a `Total` Numeric non-standard data field
will be multiplied by the number of members whereas the `Average`
Numeric non-standard data field will not.

An example of a `Total` Numeric non-standard data field might be a
salary source item (as the total salary for the group of members is
assumed) whereas an example of an `Average` non-standard data field
might be an additional contribution rate (where the same rate applies
irrespective of the number of members).

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

## Edit Num Default

Pressing the _Edit Numeric Default_ button allows Numeric Data Defaults to
be defined using an APL expression.

Note that the APL symbols may not be displayed correctly in the grid.

## Value

The entry requirement depends on its context:

module               | variable               | description
---------------------|------------------------|------------
All types            | Last Column            | Enter the length of the data record
Actives              | Salary Freq            | Enter A - annual, M - monthly, Q - quarterly, L - lunar monthly, F - fortnightly, W - weekly
Pensioners/Deferreds | If no MS, Prop Married | Enter the proportion married required
&nbsp;               | If no SDOB, Age Diff   | Enter the number of years the husband is assumed to be older than the wife. A negative number indicates the husband is younger.
&nbsp;               | Frequency of Pensions  | Enter A - annual, M - monthly, Q - quarterly, L - lunar monthly, F - fortnightly, W - weekly

## Edit Char Default

Click the _Edit Character Default_ button to modify the default value
for the character data item.

## Absolute Value

## OR Relative Value (years)

Default values for dates data items can be specified as either

-   a fixed (or absolute) date or
-   a period from the Valuation Date expressed in years (a negative
    period indicates a date prior to the Valuation Date).

The relative date avoids the need to change this date every time the
valuation date changes.

## Edit Date Default

Click the _Edit Date Default_ button to modify the default value for the
date data item.

## Edit New  Entrant Model

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