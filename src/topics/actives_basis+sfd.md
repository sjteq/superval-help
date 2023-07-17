# Spreading Finish Date for Spouse’s DIS Benefits

## Pension Benefits

If the Spouse’s Death Benefit is not insured and is either based on
Salary, Prospective Pension or Prospective Table then the user should
select whether to accrue benefits using the PUC Method or the FAS Method
in the [Spreading Method](actives_basis+stype.md).

If the FAS Method is chosen then select from the drop-down list the
Spreading Start Date. The benefit will be assumed to accrue uniformly
between the [Spreading Start Date](actives_basis+ssd.md) and the
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
Method.](actives_basis+stype.md)

If the FAS Method is chosen then select from the drop-down list the
Spreading Start Date. All of the benefit will be assumed to accrue
uniformly between the [Spreading Start Date](actives_basis+ssd.md) and
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
