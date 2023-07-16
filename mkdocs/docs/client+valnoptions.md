# Client: ValnOptions



## PPF Calculations required

Check this box to enable the user to edit the PPF parameters and run all
types of PPF valuations. This will also automatically enable the Non PPF
Capped parameters and runs. (The box will become ticked and greyed out.)

If this box is unchecked then the Relevance Rules will grey out all of
the PPF Parameters that are not used. The user will then be able to
decide whether to enable the Non PPF Capped parameters and runs
separately.

## Non-PPF Capped Calculations required

If `PPF Calculations required` has been checked then this box will
automatically be checked and greyed out. The Non PPF Capped runs
parameters will be available to edit in the Basis files and Non PPF
Capped valuations will be enabled.

If `PPF Calculations required` has not been checked then the user will
have the option to decide whether or not to enable the Non PPF Capped
parameters and runs independently. Check the box to enable these
parameters and runs. Leave the box unchecked to disable the Non PPF
Parameters that are not used in the Basis Files.

## Value Pre 1988 GMPs for Male Spouse Pensioners

Select this field to value the Pre 1988 GMPs for Male Spouse
Pensioners.

If the field is un-ticked, the Pre 1988 GMPs for Male Spouse Pensioners
will not be valued. The `VALN$.log` file will capture this.

## Use single character Basis Category when Saving Bases

This option will use the first character in the description of the
parameter set which should correspond to the category of data used if a
basis has previously been migrated from older versions. The Excel output
will then show the results by basis category.

## Analysis of Surplus Calculations required

Check this box if you require Analysis of Surplus calculations to be
carried out for this Scheme.

Entry fields relevant to Analysis of Surplus calculations are enabled or
disabled according to this selection.

## Separate Cash Commutation and Cash on Top

Tick this field to split the cash between cash commutation, cash on top
and other cash (such as Death in Service cash) in the database. This
split will be available for Actives and Deferreds. Pensioners are
already broken down by Pension 1, Pension 2, etc so the cash split was
not applied to this module.

This is only available for Users with Extended Parameters (CC3) and open
database.

## Include Individual Valuation Factors

Select this field if individual valuation factors are required in the 
Excel output and the Database. 

If this field is left blank, the individual valuation factors will
not appear in the Excel output and the Database.

## Indicate if Cash Commutation split by Pension Increase is required

If the User wishes to split the cash commutation liabilities by Pension Increases 
this field should be ticked. The results will be split in the database only. 
The Excel Output will not show the cash commutation splits by pension increases.

This cash commutation split by pension increases is possible in the Actives and 
Deferreds modules. 

To activate this field, the previous field "Separate Cash Commutation and Cash 
on Top" needs to be ticked.

## Include Year Left Service dimension

If this field is selected and entry is made in the `Future Service
Control Period` field, 2 new columns are created in the `AltScenData`
table; the LiabilityTypeID (to distinguish between Valuation and
Discontinuance Cashflows) and Year Left Service (the year the active
members have withdrawn from the Scheme).

## Use Control Period for Upper Limit of Future Service Breakdown Ranges

Select this field if the User wants to use the valuation run control
period as the Upper Limit of Future Service Breakdowns.

## Upper Limits of Future Service Breakdown Ranges

Users can define the future service breakdown in this field.

If this field is populated with e.g. `1 2 3 4 5 10 20 30 40 50 60`, the
Future Service Accrual will be split into 1, 2, 3 ,4 ,5 and then 6 – 10
will be shown under 10 years, 11 -20 be shown under 20 years etc.

If this field is set to `3 60`, then the Future Service Accrual will be a
total of 1, 2 and 3 shown under 3 and then 4 – 60 will be shown under
Future Service Accrual of 60.

## Output Separate Cash Flows for Spouse

Tick this box if separate cashflows are required for Spouses

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