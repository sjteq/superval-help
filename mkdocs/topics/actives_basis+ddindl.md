# Death in Deferment Lump Sum Benefit Basis

Select from the drop-down list what to value as a lump sum payable to a
spouse on death in deferment. The options are:

-   None
-   Return of Contributions
-   Return of Contributions if no spouse
-   Multiple of pension

If either `Return of Contributions` is selected or `Return of
Contributions if no spouse`, SuperVal will use the standard data item
AWC for contributions to the valuation date and increase this by the
member’s future service contributions specified on the Contributions
Tab. The data item for past contributions (ACW) should include interest
to the valuation date. The [ROC in Service
Interest](actives_basis+j.md) on the Contributions Tab will be used to
role up contributions until the member’s withdrawal. The [ROC in
Deferral Interest](actives_basis+jdef.md) on the Contributions Tab will
apply from withdrawal to death in deferment.

If `Return of Contributions if no spouse` is selected the benefit is
only valued for the proportion of members who do not have a spouse at
the point of death i.e. (1- Proportion Married at point of death).

If `Multiple of Pension` is selected, then SuperVal will value a
multiple of the deferred retirement pension. The Multiple is entered in
the [Multiple](actives_basis+ddlmult.md) Field.
