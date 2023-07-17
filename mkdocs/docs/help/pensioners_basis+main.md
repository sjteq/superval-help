# Pensioners Basis: Main



## Pensioner Members Data File

Double click to select the member data file containing the member data
for the particular class of membership i.e. active, deferred or pensioner.
The data file will have been created via _Data&gt;Data Build_ and will
have a `.DAT` extension. The data file will be found in the Input Folder.

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

## Use Category Selection

Click to highlight the category data you wish to use in this Basis
Category. In V9.00+ the category data can contain up to a maximum of 10
characters.

This will be useful if setting up benefit changes in addition to the
current scheme categories. For example, the user may want to run the
Category 1 data through two similar benefit categories, one with NRA 65
and one with NRA 67. The user should create a second category but select
the data for Category 1 here. The user can then make the required
changes to the rest of the benefit category.

An alternative to using the same Category Data in multiple categories
would be to create a new Basis File for the changed benefits. Most users
will find it easier to identify the purpose of the runs as the filename
can reflect the basis setup i.e. Benefit Improvements or Sale and
Purchase.

## Guarantee Period

Enter the period for which the member’s pension is guaranteed to be paid
irrespective of whether the member survives this period. For a 5 years
post retirement guarantee enter `5`. If no guarantee is payable enter `0`.

For Pensioners the remaining years guarantee period will be calculated
using the member’s standard data item `DPC - Date Pension Commenced`.

## Overlap during Guarantee Period

If the member’s pension is guaranteed, then the option to select how the
guarantee is paid becomes available.

Check this box if, on the member’s death during the guarantee period,
all outstanding payments in the guarantee period are paid as a lump sum
at death and any spouse’s reversion becomes payable immediately. When
valuing Actives or Deferreds or using the annuity calculators, the
option to select whether this benefit is discounted or undiscounted
becomes available. For Pensioners, the lump sum is calculated as the sum
of the undiscounted payments at the point of death when this option is
selected.

Leave this box unchecked if, on the member’s death during the guarantee
period, payments continue until the end of the guarantee period and any
spouse’s reversion becomes payable thereafter. Payments are always
discounted in this scenario.

## Payment Frequency

Select from the drop-down list the frequency of the pension payments.
The options are:

-   Annual
-   Semi-Annual
-   Quarterly
-   Monthly
-   Lunar-Monthly
-   Fortnightly
-   Weekly
-   Continuous

## Mode

Select from the drop-down list the timing of pension payments. The
options are:

-   In Arrears
-   In Advance

## SaveAs

Click the _Save As_ button to save with a new file name.

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