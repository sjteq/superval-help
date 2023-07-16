# Withdrawal Durational Weights

This field can be used to approximate select withdrawal rates. Double
click to select the table containing the multiplier to apply at each
duration. The duration will be calculated as the period from the
member’s Date Joined Company.

For example, a duration related table with `2` at term 0 and `1`
elsewhere would mean that the age-related withdrawal decrement was
doubled for the first year of Company service but normal thereafter.

To specify a withdrawal decrement that relates only to duration, set the
age-related withdrawal decrement to table `W001` (i.e. 1 at all ages) and
enter the decrements here.

If you do not wish to adjust for duration select the table `T000` here.
