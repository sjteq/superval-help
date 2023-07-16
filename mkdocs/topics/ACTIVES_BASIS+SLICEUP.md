# Actives_Basis+SLICEUP


## Offset Slice Number

This field is used to identify the date at which the GMP accrual
ceased.  Enter the Slice Number on which the [Service Finish
Date](actives_basis+fndate.md) should be used as the date at which GMP
accrual has ceased.  All of the benefits arising from the Slice entered
and higher Slice Numbers will be assumed to have an underlying GMP
benefit.  (Including those Slices where only added years and pension
data item benefits are specified.)

For example, if there are four Slices specified as follows:

slice | specification
------|--------------
1     | Future Service, i.e. `VDATE` to `LDATE`
2     | Service from 6/4/1997 (or `DJF` if later) to `VDATE`
3     | Service from a benefit/category change date (or `DJF` if later) to 6/4/1997
4     | Service from `DJF` to the benefit/category change date

The Offset Slice Number entered is 3, meaning that the benefits under
Slices 3 and 4 will have GMP underlying them.  The benefits under Slices
1 and 2 will not have GMP benefits.

Where the Scheme is Contracted-In and/or GMP benefits are payable on top
of the benefits entered on the Slices, enter a value of `17`.   

Please note that this field is used in a Non PPF Capped Valuation Run to
determine which parts of the pension receive pension increases.  Pension
arising from Slices before the `Offset Slice` number and higher will be
deemed to have no pension increases for PPF Valuation purposes. Pension
arising from a Slice number lower than the `Offset Slice` will be deemed
to be increasing pension in payment for PPF Valuation purposes.

