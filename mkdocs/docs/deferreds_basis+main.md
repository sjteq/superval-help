# Deferreds Basis: Main



## Deferred Members Data File

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

## Discounted LS on Death in Guarantee Period

The field is used to specify whether the Lump Sum paid as a result of a
guarantee after death is discounted or undiscounted for Actives,
Deferreds and the Annuity Calculator.

Check this box to discount, with interest, the lump sum payable. Leave
this box unchecked if the lump sum payable is undiscounted.

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

## First Year Increase

The proportion of pension increase applied in the first year is
dependent on up to 4 factors, namely:

-   When the benefit commences
-   The period between valuation and the pension increase date
-   The frequency and mode of pension payments
-   The pension increase timing.

Select from the drop-down list how the increase in the first year should
be determined. The options are:

-   Default
-   None
-   Proportional
-   Full

If "Default" is selected SuperVal assumes that, on average, people
retire halfway through the year. If the Payment Frequency is monthly,
the first pension increase will be awarded halfway through the month in
which pension increases become payable (or the review date if
specified). If the Payment Frequency is annual, first year increases are
only granted if the review date falls in the first six months after the
valuation date. The increase granted will reflect the period from the
review date to the mid-year. First year increases are not granted if the
review date falls in the second part of the first year. Subsequent
increases are valued in full on the anniversary of the commencement of
benefit. (This was the only method available prior to V8.50.)

If "None" is selected, no pension increase is valued at the first review
date or opportunity to pay pension increases following benefit
commencement.

If "Proportional" is selected, then a proportional pension increase is
valued at the first review date or opportunity to pay pension increases
following benefit commencement.

If "Full" is selected, then a full pension increase is valued at the
first review date or opportunity to pay pension increases following
benefit commencement.

## Examples

Examples illustrating how SuperVal applies pension increases under the
various methods are shown below:

Consider a £2000 annual pension payable monthly in advance from 1
January 2025. The pension increase applied is 5% p.a.

<table>
<thead>
<tr class="header">
<th>Increase Date</th>
<th>Default</th>
<th>None</th>
<th>Proportional</th>
<th>Full</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1 January</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>- First Year</td>
<td>£2000<br />
(The first increase will be given at 1 January 2026.)</td>
<td>£2000</td>
<td>£2000<br />
(The first increase will be given at 1 January 2026.)</td>
<td>£2000<br />
(The first increase will be given at 1 January 2026.)</td>
</tr>
<tr class="odd">
<td>- Second Year</td>
<td>= £2000 &times; 1.05<br />
= £2100</td>
<td>£2000<br />
(The first opportunity to pay an increase is 1 January 2026 but this is not granted hence no increase in benefit)</td>
<td>= £2000 &times; 1.05<br />
= £2100</td>
<td>= £2000 &times; 1.05<br />
= £2100</td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>1 April</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>- First Year</td>
<td>=[<sup>3½</sup>/<sub>12</sub> &times;£2000]+[<sup>8½</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2071</td>
<td>= £2000</td>
<td>=[<sup>3</sup>/<sub>12</sub> &times;£2000] + [<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>¼</sup> ]<br />
= £2018</td>
<td>=[<sup>3</sup>/<sub>12</sub> &times;£2000] + [<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2075</td>
</tr>
<tr class="odd">
<td>- Second Year</td>
<td>= £2071 &times; 1.05<br />
= £2175</td>
<td>=[<sup>3</sup>/<sub>12</sub> &times;£2000]+[<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2075</td>
<td>=[<sup>3</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>¼</sup> ]+[<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>1¼</sup> ]<br />
= £2100</td>
<td>=[<sup>3</sup>/<sub>12</sub> &times;£2000&times;1.05]+[<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05²] = £2179</td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>1 October</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>- First Year</td>
<td>= [<sup>9½</sup>/<sub>12</sub> &times;£2000]+ [<sup>2½</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2021</td>
<td>£2000</td>
<td>=[<sup>9</sup>/<sub>12</sub> &times;£2000]+[<sup>3</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>¾</sup> ]<br />
= £2019</td>
<td>=[<sup>9</sup>/<sub>12</sub> &times;£2000]+[<sup>3</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2025</td>
</tr>
<tr class="odd">
<td>- Second Year</td>
<td>= £2021 &times; 1.05<br />
= £2122</td>
<td>=[<sup>9</sup>/<sub>12</sub> &times;£2000]+[<sup>3</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2025</td>
<td>=[<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>¾</sup> ]+[<sup>3</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>1¾</sup> ]<br />
= £2100</td>
<td>= [<sup>9</sup>/<sub>12</sub> &times;£2000&times;1.05] + [<sup>3</sup>/<sub>12</sub> &times; £2000 &times; 1.05²] = £2126</td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Continuous Increases</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>- First Year</td>
<td>= [<sup>6½</sup>/<sub>12</sub> &times;£2000]+[<sup>5½</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2046</td>
<td>£2000</td>
<td>= [<sup>6</sup>/<sub>12</sub> &times;£2000]+[<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>½</sup> ]<br />
= £2025</td>
<td>= [<sup>6</sup>/<sub>12</sub> &times;£2000]+[<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2050</td>
</tr>
<tr class="odd">
<td>- Second Year</td>
<td>= £2046&times;1.05<br />
= £2148</td>
<td>=[<sup>6</sup>/<sub>12</sub> &times;£2000]+[<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05]<br />
= £2050</td>
<td>=[<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>½</sup> ]+[<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05<sup>1½</sup> ]<br />
= £2100</td>
<td>= [<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05]+[<sup>6</sup>/<sub>12</sub> &times;£2000&times;1.05²] = £2153</td>
</tr>
</tbody>
</table>

Assuming the same pension is paid annually in advance, the DEFAULT
option does not grant increases for review dates that fall after 01/07
and calculates the pension as follows:

<table>
<tbody>
<tr class="odd">
<td></td>
<td>Default</td>
</tr>
<tr class="even">
<td>1 January Increase</td>
<td></td>
</tr>
<tr class="odd">
<td>- First Year</td>
<td>£2000 (The first increase will be given at 1 January 2026)</td>
</tr>
<tr class="even">
<td>- Second Year</td>
<td>£2000 &times; 1.05 = £2100</td>
</tr>
<tr class="odd">
<td></td>
<td></td>
</tr>
<tr class="even">
<td>1 April Increase</td>
<td></td>
</tr>
<tr class="odd">
<td>- First Year</td>
<td>£2000 &times; 1.05<sup>¼</sup> = £2025</td>
</tr>
<tr class="even">
<td>- Second Year</td>
<td>£2025 &times; 1.05 = £2127</td>
</tr>
<tr class="odd">
<td></td>
<td></td>
</tr>
<tr class="even">
<td>1 October Increase</td>
<td></td>
</tr>
<tr class="odd">
<td>- First Year</td>
<td>£2000 (no increases granted as review date falls after 01/07)</td>
</tr>
<tr class="even">
<td>- Second Year</td>
<td>£2000 &times; 1.05 = £2100</td>
</tr>
<tr class="odd">
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Continuous Increases</td>
<td></td>
</tr>
<tr class="odd">
<td>- First Year</td>
<td>£2000</td>
</tr>
<tr class="even">
<td>- Second Year</td>
<td>£2000 &times; 1.05 = £2100</td>
</tr>
</tbody>
</table>

This field is only available to some users.

## Pension Benefits Capitalised or Spread

This and the other Cash Flow Parameters only affect the `Cash Flow
Summary` page in the Excel Output/Consolidation Output. They do not have
any effect on the Valuation Results.

Select from the drop-down list the option to use. The options are:

-   Capitalise
-   Spread

If `Capitalise` is selected the output will show the cashflows assuming
the benefits are capitalised at the point of first payment.

If `Spread` is selected the output will show the cashflows as they
become due.

However, the Death in Deferment Liability shown will always be the
capitalised value of the payments. The user can choose the point at
which the Death in Deferment Liability is shown in the Cash Flows
summary in the [Death in Deferment Method](actives_basis+didmethod.md)
field.

In addition, if `Spread` is chosen for Actives or Deferreds, the user
will be required to specify at which point the Underpin Liability is
capitalised in the [Underpin Method](#bases+umethod).

When running a DAB method valuation, this field must be set to
Capitalise.

## Underpin Method

This and the other Cash Flow Parameters only affect the `Cash Flow
Summary` page in the Excel/Consolidation Output. They do not have any
effect on the Valuation Results.

Where `Spread` has been chosen for the field [Pension Benefits
Capitalised or Spread](#bases+capind) the Underpin (excess) liability
will be shown as capitalised in the Cash Flow. However you can choose
where this capitalised point will be. The options are:

-   Tables
-   Default

If `Tables` is selected then enter the rate tables applicable on the
events where the Underpin is taking place. These are:

-   Retirement - actives and deferreds
-   Leaving Age - actives
-   Death in Deferment - deferreds

If `Default` is selected then the Underpin (excess) liability will be
capitalised at the payment start point.

## Retirement Age

This and the following fields affect the `Cash Flow Summary` page in the
Excel/Consolidation Output only. They do not have any effect on the
Valuation Results.

If you have selected `Tables` for the field [Pension Benefits
Capitalised or Spread](#bases+capind) then select a rate table
containing the age at which you want the Underpin (excess) liability on
Retirement to appear in the Cash Flow. The table will be indexed by age
nearest at start of the year of retirement.

Typically tables entered here would be of `EX` type.

Example Table would have entries as follows:

Age at Retirement | Age Underpin shown
------------------|-------------------
60 | 77
61 | 77
62 | 77
63 | 78
64 | 78
65 | 78

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Decr Help

Rate tables can be selected by any of the following methods:

-   Right-click on the field for a list of appropriate Rate Tables. For
    a field that will accept more than one type of Rate Table (e.g.
    Miscellaneous Tables), the list will be restricted to the current
    Table Type specified in the field – if you wish to see all allowable
    Rate Tables, delete the Table Type from the field before clicking;
    or
-   Double Clicking on the field will produce the Rate Tables form where
    Rate Tables can be viewed (numerically and graphically) and Rate
    Tables can be added or edited. A Rate Table can be selected by
    pressing the Select button or double clicking on the Rate Table
    description in the tree; or
-   the list of allowable Rate Tables can be scrolled through by
    pressing the `<` or `>` keys. The description of the Rate Table to
    the right of the field will change as each new Table is selected.

## Death Age

This and the following fields affect the `Cash Flow Summary` page in the
Consolidation Output only. They therefore do not have any effect on the
Valuation Results.

If you have selected `Tables` for the field [Pension Benefits
Capitalised or Spread](#bases+capind) then select a rate table
containing the age at which you want the Underpin (excess) liability on
Death in Deferment to appear in the Cash Flow. The table will be indexed
by age nearest at start of the year of death.

Typically tables entered here would be of `EX` type.

Example Table would have entries as follows:

Age at Leaving | Age Death Underpin shown
---------------|-------------------------
35 | 55
36 | 55
37 | 56
38 | 56
39 | 56
40 | 57
41 | 57
42 | 57
43 | 58
44 | 58
45 | 58

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Independent PUPs

Check this box to enable use of the Ind Pups Tab where details of any
Independent PUPs can be entered.

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