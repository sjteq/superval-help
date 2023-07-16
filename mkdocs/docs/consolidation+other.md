# Consolidation: Other



## Asset Value

Enter the value of the assets to be used in the consolidation of
results. The value input should be the `actuarial` value placed on the
total invested assets at the valuation date in respect of the members to
be consolidated.

## Asset Rollup Rate (% p.a.)

This is the annual rate of interest which will be used to roll up the
assets. Typically this will equal the valuation rate of interest.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this tab.

## Liability Description

## Liability Amount

Other liabilities should be used for any special liabilities which must
be calculated manually.

These other liabilities are assumed to be payable immediately and are
included in the first year cash flow on normal retirement.

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

## Scheme Fee

Scheme expenses can be expressed as a Scheme Fee which is then inflated
at a [Scheme Fee Inflation Rate](#expense_rates+expf).

The Scheme Fee will be split between different categories of active
members in proportion to their respective total salaries. Note, that
this Fee will remain unchanged (before inflation) irrespective of the
membership level and thus, for an open fund, is generally only
appropriate if a New Entrant Replacement Model is applied.

The [Member Fee (inflating per remaining
member)](#expense_rates+pmexp) can be used to represent a Scheme Fee
for an open fund where no replacement of members has been used. As the
amount for each member decreases each year as the member decrements but
the level of expense would (in theory) be maintained by new entrants to
the Scheme.

## Scheme Fee Inflation Rate (% p.a.)

This is the annual rate at which Scheme Fee will be increased.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Member Fee

Scheme Expenses can be expressed as a fixed amount (which is inflated at
the Scheme overall inflation rate) in respect of each `remaining` member
in the Scheme.

The inflating fixed amount per member is an attempt to represent a
Scheme Fee for an open fund where no replacement of members has been
used as the amount for each member decreases each year as the member
decrements but the level of expense would (in theory) be maintained by
new entrants to the fund.

## % of Company Contributions

Enter the Scheme Expenses expressed as a percentage of Company
Contributions. For 5% enter `5` not `0.05`.

Note, that the `% of Company Contributions` and the `% of Member
Contributions` fields can be used in combination to get a percentage of
total contributions.

## % of Member Contributions

Enter the Scheme Expenses expressed as a percentage of Members’
Contributions. For 5% enter `5` and not `0.05`.

Note, that the `% of Company Contributions` and the `% of Member
Contributions` fields can be used in combination to get a percentage of
total contributions.

## % of Salaries

Scheme Expenses can be expressed as a percentage of Members` salaries.
For 5% enter `5` not `0.05`.

## Edit Expenses

The _Edit Expenses_ button allows you to modify the expense assumptions if
those displayed are incorrect.

## Include Pensioners Benefits in Accrued Benefits Indices

You must specify whether you wish to include the Accrued Benefits in
respect of pensioners (both current and projected pensioners as well as
the other liabilities) in the calculation of the Accrued Benefit
indices.

## Include Insured Benefits in Cash Flow Projections

For valuation methods other than Projected Unit Credit and Unit Credit
(where the selection is made at the time of running the valuation), you
must specify whether you wish the cost of the insured benefits to be
cash flow projection.

## Graphical Presentation Only

Indicate if you wish to skip the consolidation output and simply display
the Graphical Presentation only.

## Output Full Basis Details

If you have chosen not to show a Graphical Representation Only, then you
must specify whether you wish to include the detailed basis descriptions
in the consolidation output. If unchecked, an abbreviated two page
summary is available showing the basic actuarial basis details and the
run-time of the valuation run.

## Retain Category Splits in Database

This field, when checked, differentiates different category results in
the consolidation database.

## Ignore Consolidation Descriptions for Benefit Types in Database

Indicate if you wish to ignore the Consolidation Descriptions in the
Consolidation Database

## Consolidation Output Filename

Specify the name of the file the Consolidation Output should be saved
to.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

## Use QSM Settings

User can select the parameters that are suitable for Quick Scenario Modelling 
i.e. selecting this button will set ALM/LDI Interface to "Exclude Left Servce" and tick "Retain Category Splits in Database"

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