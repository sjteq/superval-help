# PPF Details



## PPF Yields Date

Select the date containing the relevant PPF Yields specified in the PPF
Global Parameters. Where two sets of yields are stored at the same date,
use the Secondary Key to determine which set to use.

These yields will only be used in PPF runs.

To add a new set of Yields use the Edit PPF Yields button at the bottom
of this Tab.

## PPF Cap Date

Select the date containing the relevant PPF Cap information specified in
the PPF Global Parameters.

This Cap will be applied for PPF Valuation runs and also to Accrued
Benefit Liabilities in non-PPF valuation runs if requested in the
Valuation Batch parameters.

To add a new Cap use the Edit PPF Cap button at the bottom of this page.

## Service Adjusted Cap

This field is used for the PPF capping
service above 20 years. There are three options available:

Yes 

: Always apply the 3% p.a. simple increase to the cap for any service above 20 years regardless of the date

No 

: Never apply the 3% p.a. simple increase to the cap

Post 5/4/2017 Valuation Date 

: Apply the long service increase to the cap if the valuation is after 5 April 2017

## PPF Overrides Parameters

Select from the sets defined in the PPF Global Parameters the Overrides
that apply to the PPF valuation. The Overrides will contain details of
the Pre Retirement mortality and Post Retirement mortality and spouse’s
parameter overrides.

To add a new set of Overrides use the Edit PPF Overrides button at the
bottom of this Tab.

## Male Proportion Married Include Partners

## Female Proportion Married Include Partners

Check the box if SuperVal should use the proportion married including
partners as specified in PPF Guidance appropriate at the Valuation Date.
Uncheck the box if SuperVal should use the proportion married excluding
partners.

## Cap Increases Before Discontinuance

The PPF Benefit Cap can be applied to the Accrued Benefits for non-PPF
valuation runs by selecting `Cap Accrued Benefits` in the Batch
Parameters. The Benefit Cap applied will be taken from the PPF Global
Parameters and increases to the point of discontinuance with this field.
The projected Accrued Benefits page in the Consolidation output will
show the discontinuance liabilities calculated at yearly intervals
following the Valuation Date based on the projected Cap.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Cap Increases After Discontinuance

The PPF Benefit Cap can be applied to the Accrued Benefits for non-PPF
valuation runs by selecting `Cap Accrued Benefits` in the Batch
Parameters. The Benefit Cap applied will be taken from the PPF Global
Parameters. The projected Accrued Benefits page in the Consolidation
output will show the discontinuance liabilities calculated at yearly
intervals following the Valuation Date based on the projected Cap.

Select from the drop-down list the Global Financial Parameter that
contains the rate of increase relative to the net rate in deferment for
the Benefit Cap post exit. For increases in line with deferred benefits
select a Global Financial Parameter with a value of zero. Once selected,
the current value of the Global Financial Parameter is shown to the
right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Override PUP "Ignore for DBR" according to PUP PPF Service Period (Pre 1997 (Yes) and Post 1997 (No))

Users will not have to set up different bases for ongoing runs and PPF
runs when they want to override the field `Ignore the DBR` in the PUP
tab.

The highlighted field below under the PPF global parameters when ticked
will override the `Ignore for DBR` according to the PPF Service period
field described for each PUP. The Pre 1997 will be overridden to `Yes`
and the Post 1997 will be overridden to `No`.

## PPF GMP Revaluation to SPA

This is the rate at which GMP will be revalued to SPA when Fixed Rate
Revaluations do not apply and running a PPF valuation.

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected, the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the Edit Scheme Financials
button at the bottom of this Tab.

## Edit PPF Overrides

Click here to edit the PPF Override details.

## Edit PPF Caps

Click here to edit the PPF Cap details.

## Edit PPF Yields

Click here to edit the PPF Yields.

## Edit Scheme Financials

Clicking the Edit Scheme Financials button takes you to the Scheme
Financials menu.

Here you will be able to see a list of all the Financials that are
currently defined. Double-click on the tree to see an expanded list of
all financial assumptions that are defined.

Click the Add/Edit Financials to change the value of one of the
assumptions.

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