# Scenarios+TermAdjFin

Adjust financials if the defined financials are only effective at the
valuation date in the primary basis. For example if the primary basis
has a date of valuation of 31/12/2015 and the Post Retirement Interest
rate is a vector of 4%, 5%, 4.5%, 5.25%, 5%. 

If a scenario is set up with a new valuation date of 31/12/2016 and this
option is checked, the system will adjust the Post Retirement Interest
rate skipping the first rate so the adjusted vector is 5%, 4.5%, 5.25%,
5%. If this option is unchecked, the system uses the original vector.
