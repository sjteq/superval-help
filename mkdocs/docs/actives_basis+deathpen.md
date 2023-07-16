# Actives Basis: DeathPen



## Male Benefit Basis

## Female Benefit Basis

Select from the drop-down list how the death in service pension is
calculated. The options are:

-   None
-   Minimum GMP
-   Salary
-   Accrued Pension
-   Prospective Pension
-   Prospective Table

Additional fields will be required based on the option selected. The
benefits under the Accrued Pension, Prospective Pension and Prospective
Table will be based on those described on the Slices.

Not all options are available to all users.

## Male Benefit Percentage

## Female Benefit Percentage

This field is used to determine the proportion of the member’s pension
payable on death in service. This can be fixed for all members or a
member specific data item.

To use a fixed percentage for all members, enter the percentage here.
For 50% enter `50`.

To use a member specific percentage, select from the drop-down list the
data item containing the appropriate data. For 25% ensure the data
contains 25.

## Salary

An entry in this field is required if `Salary` has been selected for
either the males or females spouse’s [Death in Service Pension Benefit
Basis](#actives_basis+wobas). This field determines the Salary on
which the benefit will be based. The salary will be used rather than the
final average salary.

Select from the drop-down list one of the salaries previously specified
on the Salaries Tab.

## Pension Increases in Payment

An entry in this field is required if `Salary` has been selected for
either the males or females spouse’s [Death in Service Pension Benefit
Basis](#actives_basis+wobas). Select from the drop-down list which of
the 4 pension increase definitions should apply. The options are:

-   Main
-   Special
-   Pension Increase 3
-   Pension Increase 4.

## Male Augmentation Table

## Female Augmentation Table

An entry is required in this field if you have chosen `Prospective
Table` in either the [Ill health Pension Benefit
Basis](actives_basis+illind.md) or the [Death in Service Pension
Benefit Basis](#actives_basis+wobas). (Separate fields are available
for each of these benefits.)

Double click for a list of the available tables.

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

## Start Date for Augmentation Table

This field is required if either the males or females [Ill Health
Pension Benefit Basis](actives_basis+illind.md) or the [Death in
Service Pension Benefit Basis](#actives_basis+wobas) is based on a
Prospective Table. Select from the drop-down list the data item to use
as the date from which the benefits are augmented. (Separate fields are
available for each of these benefits.)

## Male Pension Extra Prospective Service

## Female Pension Extra Prospective Service

This field is used to increase the amount of prospective service used in
the calculation of either the ill health pension or the death in service
pension. (Separate fields are available for each of these benefits.) It
might be used where normal retirement age has been reduced post-Barber,
but the spouse’s ill health pension or death in service pension is still
based on prospective service to the member’s original normal retirement
age. Enter the number of years (and part years) additional service that
should be included. For 5 years and 6 months enter `5.5`.

## Maximum Service

## Maximum Service Table

Enter the maximum number of year’s service that can count towards
augmented ill-health pension benefits or augmented death in service
pension benefits. (A separate field is available for each benefit.)

To use a Service Maximum Table, leave the `Maximum Service` field blank
and the Maximum Service Table field will come available. Double click
for a list of available tables.

The service maximum specified for ill-health will also apply where the
Retirement Cash Option is set to `Accrual × Salary for each year` for a
retirement due to ill-health.

Some fields are only available to some users.

## CARE Death Enhancement Method

Select from the drop-down list how to value the CARE Prospective benefit
on Death in Service or Ill-health. The options are:

-   Accrued CARE Pension
-   Current Salary

The following example sets out how the benefit will be calculated under
each of these options. Consider a member with a 1/50th CARE scheme who
has a pension of £4,000 which was accrued over ten years. His current
pay is £25,000 pa. On either death or ill-health retirement he will
receive an additional 20 years of service.

Under the Accrued Care Method his death/ill-health pension will be
calculated as 

$$£4,000 + \frac{£4,000}{10} \times 20 = £12,000  $$

Under the Current Salary Method his death/ill-health pension will be
calculated as 

$$£4,000 + £25,000 \times \frac{20}{50} = £14,000$$

Some fields are only available to some users.

## Spreading Method Parameter Set

Spreading Method Parameter Set is a Scheme Global parameter which groups
the Prospective spreading method and date variables. This can be created
by using either the `Create Globals` function or using the _Add/Edit
Spreading Dates_ button. Once created, these parameters can be edited
without going back into the Basis similar to other global parameter
sets.

## Pension Spreading Method

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

## Spouse's Pension Insured

Check this box if the liability for the spouse’s Death in Service
Pension is insured with an insurance company.

Leave the box unchecked if the spouse’s Death in Service Pension
liability is valued in the pension fund. If this is selected, then you
will need to specify over what period the prospective elements are
spread.

If checked, then the [Death Pension Insured Costing
Tables](#actives_basis+wotab) will become available where you can
specify premium rate tables for SuperVal to calculate the first years
insured premium cost for this benefit.

If unchecked, define how to spread the liability.

## Male Costing Table

## Female Costing Table

If the Spouse’s Death Benefit is insured, then double click to select
the table that represents the cost of the DIS Pension benefit per
hundred pounds of pension per annum sum assured.

SuperVal will calculate the first years insured premium cost for this
benefit.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Male Rate Loading

## Female Rate Loading

If the cost of insuring a particular group of people (ie those in
hazardous occupations) is higher a loading to the standard rates can be
made. Enter the amount of the loading here. The loading should be input
as a percentage i.e. to increase the rates by 20% enter a loading of 120%.
For no adjustment enter a 100%.

Note, the insured costing for the Spouse’s Death in Service will be
costed per £100 per annum. Therefore, if this has not already been taken
account of in the premium rates (i.e. your premium rates are simply 
$qx \times ax$) you will need a rate loading of $100 \times 100% = 10,000%$.

## Male Rate Addition

## Female Rate Addition

As an alternative to a percentage loading, you can load the premium
rates by a flat amount at each age. Enter the addition to be made per
hundred pounds of pension per annum sum assured.

## Male Averaging Period

## Female Averaging Period

Specify the averaging period in years, for the Spouse’s Pension on Death
in Service insured premium.

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