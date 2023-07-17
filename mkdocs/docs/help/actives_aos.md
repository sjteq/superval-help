# Actives AOS



## Active Member Data File

Double click to select the member data file containing the member data
for the particular class of membership i.e. active, deferred or pensioner.
The data file will have been created via _Data&gt;Data Build_ and will
have a ` extension. The data file will be found in the Input Folder.

## Data Format

Double click to select the Format File for the current Data File. The
Format File contains the saved parameters specifying the column
specification of each of the data items contained in the data file. Data
format descriptions are prefixed by an indication of the type of format
e.g. &lt;Act&gt; for Actives, &lt;Def&gt; for Deferreds, &lt;Pen&gt; for Pensioners.

If you intend to use the GMP Calculators to calculate GMPs after
creating your data, ensure that columns are created in your data file
for these fields. (In addition, enter dummy data into the data file for
the first member that is at least as large as the largest expected GMP
for all members. This will ensure that the Format created leaves
sufficient space for the GMPs calculated.)

## Data&gt;Build

If you have created data using _Data&gt;Build_ then the format name will
be the same as the original source (CSV) file.

## BasisModule&gt;Migrate

If you have migrated your data files from earlier versions the name will
be unchanged.

## Entry Based on Date of Joining

This field is used to separate the results of the Analysis between
members at the previous valuation date (Old) and new entrants since the
previous valuation (Starters). Select from the drop-down list whether to
split based on Company Service or Scheme Membership. The options are:

-   Scheme
-   Company

If Scheme is selected the age at entry will be determined from the
standard data item DJF (Date Joined for Pensionable Service). If Company
is selected the age at entry will be determined from the standard data
item DJS (Date Joined for Company Service).

## Set Retrospective Reserve at Entry to zero

For valuation methods that use a retrospective reserve (that is,
Attained Age Normal, Projected Unit Credit and Defined Accrued Benefit
methods), you are able to specify whether the Reserve should be zero for
new entrants at entry.

Leave this field unchecked if new entrants are able to transfer in
periods of membership or additional pension amounts, when a non-zero
Reserve at Entry would be expected.

Check this field if all new entrants have no previous fund accruals.

Note that the Reserve calculated by the system for new entrants with no
previous fund accruals only differs from zero due rounding in the
interpolation between Reserves.

## Flag indicating sufficient Previous Data

This field enables you to specify a non-standard numeric data field that
indicates whether sufficient data exists to be able carry out Reserve
calculations at the Previous Valuation Date or Entry (if later).

If the specified data field is zero (or blank) then no Reserve
projections will be carried out (and the approximations will apply).

For example, if contributions information is available but salary
information is not, SuperVal would derive a Reserve based upon
contributions benefits only as the salary benefits would be zero (as
SuperVal is not intelligent enough to know if a data field should not be
zero!)

The specified data field may be a field especially for this purpose.

## Flag indicating sufficient Current Data

This field enables you to specify a non-standard numeric data field that
indicates whether sufficient data exists to be able carry out Reserve
calculations at the Current Valuation Date or Exit (if earlier).

If the specified data field is zero (or blank) then no Reserve
projections will be carried out (and the approximations will apply).

For example, if contributions information is available but salary
information is not, SuperVal would derive a Reserve based upon
contributions benefits only as the salary benefits would be zero (as
SuperVal is not intelligent enough to know if a data field should not be
zero!)

The specified data field may be a field especially for this purpose.

## Retirement

## Death In Service

## Ill-Health

## Withdrawal

For each cause of exit, select the codes that identify members who have
exited from that cause. Any number of modes of exit can be specified to
represent each of the different causes of exit.

## Save

Clicking on the _Save_ button allows you to save the entries.

## Quit

Clicking on the _Quit_ button allows you to exit without saving any of
your changes.

In some of the screens you will be asked to confirm if you want to exit
_Ignoring all changes_. If you click _Yes_, the file will be closed
without saving any changes. If you click _No_ you will be returned to your
original screen.

From the Browser, the _Quit_ button will take you to a graphical display
of the results.