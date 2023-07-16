# Quick Scenario: Demographic



## Consolidation Database File

Select the database file containing the results to run the Quick
Scenario Modeller on i.e. the _original_ results in the graphs /
output.

## Consolidation SQL Server Database

Select the consolidation SQL server database file to be used for QSM

## Type of Graph

The default is _liabilities_. Choose to view one of the following 7
options:  

-   Liabilities – these are split into membership groups (actives / deferreds / pensioners) and      past and future service
-   Waterfall Liabilities  
-   Financial Position  
-   Waterfall Financial Position  
-   Cash Flows  
-   Employer Contributions  
-   Employer Funding Rate

## Term

The term displayed for the cashflows i.e.in the graphs _Cash Flows_,
_Employer Contributions_ and _Employer Funding Rate_ can be adjusted
here to display the results for the term required.

## Membership Groups

Membership Groups  

Select from:  

-   All
-   Active
-   Deferred
-   Pensioner
-   Active / Deferred
-   Deferred / Pensioner
-   Active / Pensioner

## Contributions

Contributions checkbox appears as an option if employee contributions
have been included   
within the Actives basis. These will then be included within the
cashflow graphs / output.

## Expenses

Expenses checkbox appears as an option if expenses have been included
when running the consolidation. These will then be included within the
cashflow graphs / output.

## Additional Liabilities

Additional Liabilities checkbox appears if additional liabilities have
been included when running the consolidation.  These will then be
included within the cashflow graphs / output.

## Post-Retirement Mortality Adjustment

If, under File &gt; Properties &gt; Valn Options the box _Output Separate
Cashflows for Spouse_ is ticked, then it is possible to adjust the
post-retirement mortality.  
  
If the _per Annum_ box is unchecked then mortality will be adjusted
overall by the percentage specified. A number or a vector can be input here.

## per Annum from the Valuation Date

If the _per Annum_ box is checked then the mortality adjustment will be
applied to the mortality improvement i.e. by
$(1 - mortality adjustment)^{t}$ at time $t$.

## Proportion Married Adjustment

Specify the Proportion Married Adjustment.

## Configure Roll-Forward

Configure Financial Assumptions for Roll-Forward Valuations 
i.e. whether discount rates / escalation rates and adjustments to these apply from  Valuation Date or Roll-Forward Date.

## Create Financials

A new set of Financial assumptions can be created for the changes that have been input in the Financial tab.

## Dump Results

Selecting _Dump Results_ in the bottom right of the screen will produce
a TXT file.
  
This contains the:  

-   adjustments to the financials/mortality  
-   original / change in / revised liabilities, split by benefit type  
-   revised cashflows, split into components (e.g. Ret Pen / Ret Cash / Death Pen / Death Cash)

## Amortise Deficit

If amortisation is included when consolidating, then selecting _Amortise
Deficit_ will adjust the amortisation assumptions to amortise any
surplus / deficit.  
  
A new box will appear asking which amortisations are to be included:  
  
-   Both Amortisations  
-   Amortisation 1  
-   Amortisation 2  
  
and which of the two currently variable fields out of rate / term /
amount (one has previously been chosen to be constant) is to change to
amortise the surplus / deficit.  

If _Both Amortisations_ is chosen then a further box _Shared_ will be
displayed with a choice between sharing between the two amortisation
methods equally or proportionally.

## Configure Graphs

Choose type of bar chart for cash flows.

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