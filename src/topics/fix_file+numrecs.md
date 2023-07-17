# Limit Number of Records in Fixed File

Specify the number of records to be included in the `fixed` file. Leave
blank if you wish all records to be included in the `fixed` file.

This feature can be used to either:

-   create a test data file with only a few records used for testing
    the results of some calculations; or
-   remove any unwanted records added by the Fixing program by
    specifying the expected number of records in the file. (The Fixing
    program will add another record if any characters (which may be only
    end of file markers) are found beyond the last record.)
