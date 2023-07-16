# Actives Basis: DeathCash



## Return of Contributions

Select from the drop-down list what benefit to value as a Return of
Contributions on Death in Service. The options are:

-   Nothing
-   Member’s Contributions
-   Money Purchase Underpin

This is payable in addition to the other benefits specified for death in
service.

## Multiple

Enter the multiple of salary that is paid as a lump sum on death in
service.

## Of Salary

Select from the drop-down list the salary to use in the calculation of
the Lump Sum on death in Service. All of the salaries previously
specified on the Salaries Tab should be available.

## Spreading Method Parameter Set

Spreading Method Parameter Set is a Scheme Global parameter which groups
the Prospective spreading method and date variables. This can be created
by using either the `Create Globals` function or using the _Add/Edit
Spreading Dates_ button. Once created, these parameters can be edited
without going back into the Basis similar to other global parameter
sets.

## Cash Spreading Method

If the benefits are not insured, this field is used to determine how the
accrual of either a salary related or a prospective pension or cash
benefit is spread. Select from the drop-down list which of the following
options to use:

-   FAS
-   Projected Unit

For CC3 users the selection on the Death Pen Tab will be used for both
pension and cash benefits paid on death.

The `FAS` option values the full prospective element whenever the member
is assumed to exit, then spreads this over the period from [Spreading
Start Date](#actives_basis+ssd) to [Spreading Finish
Date](#actives_basis+sfd). For normal FAS values, Spreading Start
Date should be set to DJF and Spreading Finish Date to LDATE.

The `Projected Unit` option values the full prospective element for
those who exit within the control period only. For those who do not exit
during the control period, only the benefit based on accrued service is
valued. Spreading dates are ignored. For attained age valuations,
SuperVal values the full prospective element for all future exits, i.e.
the control period is infinite.

Not all options are available to all users.

## Spreading Start Date

## Pension Benefits

If the Spouse’s Death Benefit is not insured and is either based on
Salary, Prospective Pension or Prospective Table then the user should
select whether to accrue benefits using the PUC Method or the FAS Method
in the [Spreading Method](#actives_basis+stype).

If the FAS Method is chosen then select from the drop-down list the
Spreading Start Date. The benefit will be assumed to accrue uniformly
between the Spreading Start Date and the [Spreading Finish
Date](#actives_basis+sfd) and is split between past and future
service on the same uniform basis.

If the pension is % of salary then the whole of the benefit is
apportioned between past and future service liability.

For the Prospective Pension or the Prospective Table it is the
prospective element only that is spread. (The pension from service prior
to the valuation date will be valued as past service. The pension from
service between the valuation date and the point of exit will be future
service liability. The pension from service between point of exit and
NRD is spread between the dates entered.)

The past service liability will be equal to:

$$\frac{(SD to VDATE) \times Prospective Element}{SSD to SFD}$$

<!-- 
<table>
<tbody>
<tr class="odd">
<td></td>
<td>SD to VDATE</td>
<td>x Prospective Element</td>
</tr>
<tr class="even">
<td></td>
<td>SSD to SFD</td>
<td></td>
</tr>
</tbody>
</table>
 -->
The future service liability will be equal to:

$$\frac{(VDATE to SFD) \times Prospective Element}{SSD to SFD}$$

<!-- 
<table>
<tbody>
<tr class="odd">
<td></td>
<td>VDATE to SFD</td>
<td>x Prospective Element</td>
</tr>
<tr class="even">
<td></td>
<td>SSD to SFD</td>
<td></td>
</tr>
</tbody>
</table>
 -->
where:

-   SSD = Spreading Start Date  
-   SFD = Spreading Finish Date  
-   VDATE = Valuation Date


### Lump Sum Benefits

If the Lump Sum on Death Benefit is not insured and is a multiple of
Salary then the user should select whether to accrue benefits using the
PUC Method or the FAS Method in the [Spreading
Method](#actives_basis+stype).

All of the benefit will be assumed to accrue uniformly between the
Spreading Start Date and the [Spreading Finish
Date](#actives_basis+sfd) and is split between past and future
service on the same uniform basis.

The past service liability will be equal to:

$$\frac{(SD to VDATE) \times Multiple \times Salary}{SSD to SFD}$$

<!-- 
<table>
<tbody>
<tr class="odd">
<td></td>
<td>SD to VDATE</td>
<td>x Multiple &times; Salary</td>
</tr>
<tr class="even">
<td></td>
<td>SSD to SFD</td>
<td></td>
</tr>
</tbody>
</table>
 -->
The future service liability will be equal to:

$$\frac{(VDATE to SFD) \times Multiple \times Salary}{SSD to SFD}$$

<!-- 
<table>
<tbody>
<tr class="odd">
<td></td>
<td>VDATE to SFD</td>
<td>x Multiple &times; Salary</td>
</tr>
<tr class="even">
<td></td>
<td>SSD to SFD</td>
<td></td>
</tr>
</tbody>
</table>
 -->
where:

-   SSD = Spreading Start Date  
-   SFD = Spreading Finish Date  
-   VDATE = Valuation Date

Not all options are available to all users.

## Spreading Finish Date

## Pension Benefits

If the Spouse’s Death Benefit is not insured and is either based on
Salary, Prospective Pension or Prospective Table then the user should
select whether to accrue benefits using the PUC Method or the FAS Method
in the [Spreading Method](#actives_basis+stype).

If the FAS Method is chosen then select from the drop-down list the
Spreading Start Date. The benefit will be assumed to accrue uniformly
between the [Spreading Start Date](#actives_basis+ssd) and the
Spreading Finish Date and is split between past and future service on
the same uniform basis.

If the pension is % of salary then the whole of the benefit is
apportioned between past and future service liability.

For the Prospective Pension or the Prospective Table it is the
prospective element only that is spread. (The pension from service prior
to the valuation date will be valued as past service. The pension from
service between the valuation date and the point of exit will be future
service liability. The pension from service between point of exit and
NRD is spread between the dates entered.)

The past service liability will be equal to:

$$\frac{(SD to VDATE) \times Prospective Element}{SSD to SFD}$$

The future service liability will be equal to:

$$\frac{(VDATE to SFD) \times Prospective Element}{SSD to SFD}$$

where:

-   SSD = Spreading Start Date
-   SFD = Spreading Finish Date
-   VDATE = Valuation Date


## Lump Sum Benefits

If the Lump Sum on Death Benefit is not insured and is a multiple of
Salary then the user should select whether to accrue benefits using the
PUC Method or the FAS Method in the [Spreading
Method.](#actives_basis+stype)

If the FAS Method is chosen then select from the drop-down list the
Spreading Start Date. All of the benefit will be assumed to accrue
uniformly between the [Spreading Start Date](#actives_basis+ssd) and
the Spreading Finish Date and is split between past and future service
on the same uniform basis.

The past service liability will be equal to:

$$\frac{(SD to VDATE) \times Multiple \times Salary}{SSD to SFD}$$

The future service liability will be equal to:

$$\frac{(VDATE to SFD) \times Multiple \times Salary}{SSD to SFD}$$

where:

-   SSD = Spreading Start Date
-   SFD = Spreading Finish Date
-   VDATE = Valuation Date

Note: Not all options are available to all users.

## Lump Sum Insured

Check this box if the liability for the Lump Sum on Death in Service is
insured with an insurance company. Leave this box unchecked if the
liability for the Lump Sum on Death in Service is paid from the pension
fund.

If checked, then [Death Insured Costing Tables](#actives_basis+gltab)
become available where you can specify premium rate tables for SuperVal
to calculate the first years insured premium cost for this benefit.

If unchecked, define how to spread the liability.

## Male Costing Table

## Female Costing Table

If the Lump Sum Death Benefit is insured, then double click to select
the table that represents the cost of the Lump Sum benefit per thousand
pounds sum assured.

SuperVal will calculate the first years insured premium cost for this
benefit.

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

## Male Rate Loading

## Female Rate Loading

If the cost of insuring a particular group of people (i.e. those in
hazardous occupations) is higher a loading to the standard rates can be
made. Enter the amount of the loading here. The loading should be input
as a percentage i.e. to increase the rates by 20% enter a loading of 120%.
For no adjustment enter a 100%.

Note, the insured costing for the Lump Sum on Death in Service will be
costed per £1,000 per annum. Therefore, if this has not already been
taken account of in the premium rates (i.e. your premium rates are
simply `qx`) you will need a rate loading of 100 &times; 1000 % = 100,000%.

## Male Rate Addition

## Female Rate Addition

This field allows an addition of a flat amount to the rate at each age
to be made. Thus increasing the insured cost of this benefit. Enter the
addition here.

The addition will be in terms of per hundred pounds of lump sum assured.

## Male Averaging Period

## Female Averaging Period

Specify the averaging period in years, for the Lump Sum on Death in
Service insured premium.

An entry for averaging period may be necessary if some smoothing of the
insured premium rates is required.

## Linearly Interpolate Costing Tables for mid-point Exit values

When checked, the system will linearly interpolate factors for mid year
exits such as early retirements and deaths. For Normal Retirements, the
system will apply no interpolation. If unchecked, the system will use
the factor specified at the age nearest rounded down for mid year exits
as previous versions have done.

## Add/Edit Spreading Dates

Add or Edit any Spreading Date parameter sets.

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