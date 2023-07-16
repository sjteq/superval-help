# Revaluation Rate to NRA&lt;SPA

This is the rate at which GMP benefits will be revalued to NRA if the
[Revalue to NRA&lt;SPA](actives_basis+gmpdefind.md) box has been
checked. At SPA, SuperVal will revalue the GMP using the [Revaluation
Type to SPA](actives_basis+grev.md) selected. Any shortfall in
revaluations (when compared to the GMP at NRA) will be added to the PUP
at SPA. The addition at SPA would be subject to the [Franking
Code](bases+offcod.md).

Select from the drop-down list the Global Financial Parameter that
contains the rate applicable. Once selected the current value of the
Global Financial Parameter is shown to the right of this field.

To add a new Global Financial Parameter use the _Edit Scheme Financials_
button at the bottom of this Tab.

An example to illustrate this is set out below:

Suppose you have a male member who is currently 30 who will retire at
age 60. All of his pension is revalued in deferment at 3.5% pa. The user
has checked the Revalue to NRA&lt;SPA box and has selected a Global
Financial Parameter with a value of 3.5% for this field. The GMP
revaluation type is fixed. The pension accrued in the 2nd year is £1,000
of which £500 is GMP. Once in payment, the pension will increase at 4%
per annum.

The deferred PUP payable at age 60, after leaving in the second year,
will be calculated as 

$$ £1,000 \times 1.035^{28} = £2,620 $$

(Note that GMP is revalued using complete years in the same way
as the excess over GMP.)

The addition at SPA for GMP revaluations not yet in payment, assuming no
franking, is calculated as 

$$£500 \times 1.045^{32} - £500 \times 1.035^{28} = £735$$

(Note that complete tax
years are used for the revaluation of the GMP to SPA.)

The deferred PUP at SPA will be calculated as 

$$£2,620 \times 1.04^5 + £735 = £3,923$$
