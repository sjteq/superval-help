# Output Data Field

You must specify the start and end columns (both inclusive) of the
output data field where the calculated result is to be inserted in the
data records.

This field can overwrite an existing data field in the records
(including one of the input data fields from which the result is being
calculated).

If necessary, the output data field may be beyond the end of the member
record and the member data records will be lengthened to accommodate the
field (including moving the last column which fixes the length of the
records). Note that it will be necessary to modify the data format if
this is done.

Ensure you specify sufficient columns to fit the largest possible result
(including the decimal point, if any) as an error will be reported if
all results do not fit.
