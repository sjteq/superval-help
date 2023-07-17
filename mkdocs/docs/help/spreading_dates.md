# Spreading Dates



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