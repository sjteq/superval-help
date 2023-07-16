# Formula for Calculated Data Field

The formula to calculate the value of the calculated input data field is
specified in APL Coding. The values contained in the data fields should
be specified as:

-   FV1, FV2 and FV3 for the three numeric input data fields
    respectively;
-   FV4 for the character input data field; and
-   FV5 and FV6 for the two input date fields respectively.

In addition to the functions that can be used in coding of benefits, the
following functions are also available:

`date1 DATEMAX date2` 

: the result is the later of the two dates specified (either of which may be fixed date expressed in DD MM YYYY)

`date1 DATEMIN date2`

: the result is the earlier of the two dates specified 
	(either of which may be fixed date expressed in DD MM YYYY)

`days DATEOFFSET date` 

: the result is the date offset by the number of days.

This formula is checked (as far as possible) for syntax etc. before the
run is executed.
