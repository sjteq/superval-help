# Rates

The values in the Rate Table are displayed and can be modified in the
`spreadsheet`.

The range of Rates that can be specified are:

-   pages 0 to 119 for Age-related Rate Tables (including Miscellaneous
X-tables)

-   durations 0 to 59 for Duration related Rate Tables (including
Miscellaneous T-tables);

-   dimensions of up to 120 values (related to Age (Y-axis) and Duration
(X-axis) for decrement rates) for 2-Dimensional Rate Tables (including
Miscellaneous M tables); and

-   ages 0 to 119 and durations 0 to {select period +1} for Select Rate
Tables. The mortality suffered by an individual member follows a
diagonal of the table so the Rates entered at each age (i.e. a row) for a
$t$-year select period are 

        q[x]:0, q[x-1]:1, q[x-2]:2, ..., q[x-t+1]:t-1, qx{Ultimate}

Only one column of Ultimate rates should
be specified as all durations beyond `t` year select period will use the
Ultimate rates column.

The format of the Rates being entered will depend on the type of Rate
Table being entered (an `out of range` error will be reported if an
invalid entry is input). It is necessary to input decimal points.

## Duration-related 2D tables

To determine the age used to look up the factor in Duration-Related
Decrement Tables, SuperVal will calculate both the Age Exact and the
Age Nearest at the start of the year. If Age Exact is less than Age
nearest, SuperVal will use the Age Nearest to look up the decrement at
point of exit. If Age Exact is greater than (or equal) to Age Nearest,
SuperVal will use the Age Nearest + 1 to look up the decrement at point
of exit.

To determine the service used to look up the decrement, SuperVal will
calculate the period from Date of Entry into Qualifying Service/Start
Date for Augmentation Table and anniversary of valuation date +1.
