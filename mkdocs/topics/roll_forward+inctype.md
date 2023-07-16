Select the Escalation Method:


None

: This option will apply no escalation to the Data Field.

: Fields required: None


Interest/Revaluation

: This will perform a simple roll-up at the rate specified in the
‘Escalation Rate’ column for the Roll Forward period.

: Fields required: Escalation Rate

: Where (assumed continuous increases).


Increases

: The method of escalating the data field will depend on which `Escalation Timing` is specified.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`)


Escalation Rate

: If Escalation Timing is Continuous, the same calculation will be applied as in Interest/Revaluation above. If the timing is Review Date, a full year’s increase will be applied on each Review Date within the Roll Forward period.


Inflation

: The same calculation will be applied as for Increases but with the inclusion of any Promotional Salary Increases.

: Fields required: `Salary Scale` (Male and Female), `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Escalation Rate`


Age Dependent

: This method of escalating the data field will depend on the Payment Start Age specified.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Payment Start Age` (Male and Female), `Age Dependent Revaluation`


Age-Dependent Increases

: Revaluation will be applied prior to the Payment Start Age and Increases will be applied after the Payment Start Age. The calculation is described in Revaluation and Increases above.


Excess over GMP

: This calculation is similar to Age Dependent above but allowing for the GMP.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Payment Start Age` (Male and Female), `Age-Dependent Revaluation`


Age-Dependent Increases

: The formula is:


If Not Fixed

: The calculation is applied as for Age Dependent if GMP Fixed Revaluation is not checked. If GMP Fixed Revaluation *is* checked: substitute Fixed Revaluation Rate (see above) if it is GMP Fixed Revaluation.

: Fields required: `Escalation Timing`, `Review Date` (if Escalation Timing is `Review Date`), `Payment-Start Age` (Male and Female), `Age-Dependent Revaluation`
