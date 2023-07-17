# Past GMP Revaluation Rate(s) to NRA&lt;SPA Factor Set

This field only applies to normal/early retirement pensions before SPA.
It is not used for death in deferment benefits. If GMP retirement
benefits payable before SPA are determined using a different rate of
revaluation to that used to SPA then the past Revaluation Rates should
be entered here.

SuperVal will roll back the GMP at valuation date to GMP as at date of
leaving active service using either [Fixed Revaluation Rate to SPA](deferreds_basis+gmprev2.md)
or [Revaluation Rate to SPA](deferreds_basis+gmprev1.md) as applicable.
SuperVal will then roll forward the GMP to NRA using the rate(s) specified
here. Therefore, if an entry is made in this field the data item containing
the date of leaving active service must be specified in the [Date Left Active](deferreds_basis+leaving.md)
on the Membership Tab.

Select from the drop-down list the Factor Table Set that contains the
applicable past Revaluation rates.

Note that the Factor Table Set consists of a series of Increase Dates and
Revaluation Rates (%).  The values are NOT cumulative (this differs from
the Factor Table Set currently in use for [Pre Valuation Date Factor Set](deferreds_basis+revset.md)).
Any Increase Dates that fall between a members' Leaving Date and the 
Valuation Date will be included (in full) in the past Revaluation Rates.