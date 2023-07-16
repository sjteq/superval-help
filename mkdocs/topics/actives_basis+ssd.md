# Spreading Start Date for Spouse’s DIS Benefits

## Pension Benefits

If the Spouse’s Death Benefit is not insured and is either based on
Salary, Prospective Pension or Prospective Table then the user should
select whether to accrue benefits using the PUC Method or the FAS Method
in the [Spreading Method](actives_basis+stype.md).

If the FAS Method is chosen then select from the drop-down list the
Spreading Start Date. The benefit will be assumed to accrue uniformly
between the Spreading Start Date and the [Spreading Finish
Date](actives_basis+sfd.md) and is split between past and future
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
Method](actives_basis+stype.md).

All of the benefit will be assumed to accrue uniformly between the
Spreading Start Date and the [Spreading Finish
Date](actives_basis+sfd.md) and is split between past and future
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
