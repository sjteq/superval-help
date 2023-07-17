# The Import Rates button

Pressing the _Import Rates_ button enables importing rates from an ASCII
file.

The standard Windows dialog box is presented allowing you to select a
file containing the rates to be imported.

The file can be either a Text file or CSV (Comma Separated Values) file
and should contain

-   for Age and Duration related Rate Tables, a series of numbers being
alternate values of Age/Duration followed by a Rate (similar to the
`.TAB` export files created by SuperVal)
-   for 2-Dimensional Tables, a series of records containing Rates for
each respective Age (or Y-axis dimension).

It is not necessary to specify a rate for every Age and/or Duration in
the file as the default value will be assumed (one for Duration
related tables and zero for all other tables) for any unspecified
Ages/Durations.

However, the file is assumed to contain Rates for all Ages and/or
Durations so all existing rates in the Rate Table are replaced by the
imported rates.

After accepting the parameters, the effect of the import is displayed
for confirmation before the Rate Table is updated.

More information can be found in the Infocus document relating to
Importing of Rate Tables.
