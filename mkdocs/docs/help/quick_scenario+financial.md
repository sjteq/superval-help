# Quick Scenario: Financial



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

## Relative Change

## New Values

## % Change

## % of Current Values

﻿

Variations can be:  

Relative Change 

An absolute addition or subtractive relative to the current financial assumptions  

New Values 

These overwrite the current financial assumptions  

% Change 

New financial assumption is: (1+% input) &times; current financial assumptions

% of Current Values 

New final assumption is: % input &times; current financial assumptions

## Rate 1 Description

## Rate 2 Description

## Rate 3 Description

## Rate 4 Description

## Rate 5 Description

## Rate 6 Description

## Rate 7 Description

## Rate 8 Description

## Rate 9 Description

## Rate 10 Description

## Rate 11 Description

## Rate 12 Description

## Rate 13 Description

## Rate 14 Description

## Rate 15 Description

Adjustments:  
  
Here adjustments can be made to the groups set up within the Scheme
Financial Assumptions, subject to a minimum of -10 and a maximum of +10.
Note the percentage is input here e.g. `1` rather than `0.01`.  
  
Adjustments can be:  

-   A single number, which can be negative or positive  
-   A vector of numbers, separated by a space or a comma (limit of 25 digits)
-   A yield curve (CSV file)

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