# Service Related Accrual Table

This is `ET`, `FT`, `GT` and `HT` type rate tables, which is indexed by
the period of service specified by the Benefit Slice. It is the
corresponding entry on the `ET`, `FT`, `GT` and `HT` table that is used
in the benefit calculation.

The service period is calculated from [DOE Qualifying
Service](actives_basis+doeqs.md) to the start date/end date on the
slice. SuperVal will then linearly interpolate to obtain the value for
the member’s exact period of service.

Typical uses for this table may be uplifted service or extra years of
service granted after a certain period. For example, suppose that
members receive a further 5 years pensionable service on completion of
10 years. The Service Related Accrual Table would have an entry of `9` at
duration 9 and `15` at duration 10, `16` at 11 etc. i.e. the table is
cumulative.

Please note that the Service Related Accrual Table will be applied
across Benefit Slices (or Tiers).

If a `ET`, `FT`, `GT` and `HT` table is not defined, then the service
will be the period between the Start Date (or minimum start date) and
Finish Date (or maximum finish date) for the Benefit Slice. Allowance
would be made for maximum service.

Double click to select from the list of available `ET`, `FT`, `GT` and
`HT` type rate tables.

When using this field, you will be required to enter the date from which
service starts to accrue in the [DOE Qualifying
Service](actives_basis+doeqs.md) on the Membership Tab.

Not all functionality is available to all users.
