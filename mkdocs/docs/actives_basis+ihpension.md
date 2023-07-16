# Actives Basis: IHPension



## Male Benefit Basis

## Female Benefit Basis

Select from the drop-down list how the ill-health pension is calculated.
The options are:

-   None
-   Accrued Pension
-   Prospective Pension
-   Prospective Table

Additional fields will be required based on the option selected. The
benefits under the Accrued Pension, Prospective Pension and Prospective
Table will be based on those described on the Slices.

Not all options are available to all users.

## Male Future Service Fraction

## Female Future Service Fraction

This is used where the Ill health [Benefit
Basis](#actives_basis+illind) is a Prospective Pension.

If the prospective service is to count in full then this field should be
set to 100%. If prospective service only counts at half rate then this
field should be set to 50%.

More information on how the cost of the prospective element is accrued
is found in the [Spreading Method](#actives_basis+stype) and
[Spreading Dates](#actives_basis+ssd).

## Male Reduction Factors

## Female Reduction Factors

This field allows the user to specify a set of early retirement
reduction factors that apply to ill health pension benefits. Typically,
where these are unreduced the factors would be 1 at all ages. Double
click to select from the list of available tables.

If the field is left blank then SuperVal will assume 1 at all ages.

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

## Linearly Interpolate Reduction Factors for mid-point Exit values

When checked, the system will linearly interpolate factors for mid year
exits such as early retirements and deaths. For Normal Retirements, the
system will apply no interpolation. If unchecked, the system will use
the factor specified at the age nearest rounded down for mid year exits
as previous versions have done.

## Male Augmentation Table

## Female Augmentation Table

An entry is required in this field if you have chosen `Prospective
Table` in either the [Ill health Pension Benefit
Basis](#actives_basis+illind) or the [Death in Service Pension
Benefit Basis](actives_basis+wobas.md). (Separate fields are available
for each of these benefits.)

Double click for a list of the available tables.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Start Date for Augmentation Table

This field is required if either the males or females [Ill Health
Pension Benefit Basis](#actives_basis+illind) or the [Death in
Service Pension Benefit Basis](actives_basis+wobas.md) is based on a
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

## Apply Reduction Factor to Spouse's

Check this box if the spouse’s pension payable on ill health retirement
should include the ill-health reduction factor tables specified. Leave
this box unchecked if the spouse’s pension is unreduced.

## Spouse's Based on Pre Commutation Pens

Check this box if the spouse’s pension payable on ill health retirement
should be based on the member’s pre-commutation pension. Leave this box
unchecked if the spouse’s pension is based on the post-commutation
pension.

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

## CARE Ill-Health Enhancement Method

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

## Spreading Method

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