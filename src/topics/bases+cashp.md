# Cash Commutation Priority

This field is used to determine the order in which pension will be
commuted for cash. Select from the drop-down list which of the options
to use. The options are:

-   After Split (actives only)
-   Before Split (actives only)
-   Priority
-   Pro Rata

If `After Split` or `Before Split` is used then the pension is commuted
by reference to the `Latest Finish Date` specified on the [Offset
Slice](actives_basis+sliceup.md).

Typically an active member will have a service timeline as shown in the
following diagram:

![](img/bm6.gif)

If `After Split` is selected then the pension accrued after the End of
the Offset Slice would be commuted first. Within each period pension may
increase at different rates and are commuted in the following order:

-   Special
-   Main
-   Pension Increase 3
-   Pension Increase 4

If `Before Split` is selected then the pension accrued before End of the
Offset Slice would be commuted first. Within each period pension may
increase at different rates and are commuted in the following order:

-   Special
-   Main
-   Pension Increase 3
-   Pension Increase 4

If `Priority` is selected then the cash is commuted according to the
pension increase rate applied on the Slices or PUP Tab. Pensions are
commuted in the following order:

-   Special
-   Main
-   Pension Increase 3
-   Pension Increase 4

If `Pro Rata` is selected, then pension is commuted in proportion to the
pension amounts, irrespective of the pension increase rate.
