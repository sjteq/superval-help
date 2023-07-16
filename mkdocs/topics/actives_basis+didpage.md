# Death in Deferment: Pension

This field is only used to position the results in the `Cash Flow
Summary` page in the Excel/Consolidation Output. It does not have any
effect on the Valuation Results.

If you have selected `Tables` for the [Death in Deferment
Method](actives_basis+didmethod.md) then double click to select the
rate table containing the age at which you want the Death in Deferment
Pension Liability to be capitalised in the Cash Flow Summary. The table
will be indexed by age nearest at start of the year of death.

For example, a Table assuming the liability will be capitalised 2/3rds
of the way to retirement at age 65 would have entries as follows between
35 and 45:

Age at Start of the Year of Leaving | Age DID Pension Capitalised Value Shown
------------------------------------|----------------------------------------
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


The figure appearing in the Cash Flow Summary Listing will be the
capitalised Death in Deferment Pension liability rolled forward with
interest. The roll forward is taken from the assumed exit (half way
through the year) to the start of the year that the member will be the
age (nearest) to the corresponding entry in the table i.e. a roll forward
with interest for the term `Age DID Pension Capitalised Value Shown`
less `Age at Start of Year of Leaving` less 0.5.
