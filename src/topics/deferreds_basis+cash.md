# Cash Commutation: Multiple/Percentage

The commuted cash can be calculated either as a Multiple or a Percentage
of the PUP.

If an entry is made in the Multiple field, the commuted cash will be
calculated as:

Multiple &times; PUP revalued to retirement &times; Early Retirement Reduction
Factor (if applicable).

The Multiple can either be a fixed Multiple for all members or a Member
Specific Multiple. To use a fixed Multiple enter the value i.e. for 4
times the PUP enter `4`. To use a Member Specific Multiple, select from
the drop-down list the data item containing the appropriate value. To
value commutation of 4 times the PUP ensure the data item contains the
value 4.

To value a Percentage, ensure the entry in the Multiple field is blank.
The commuted cash can be calculated as:

Percentage &times; PUP revalued to retirement &times; Commutation Factor &times; Early
Retirement Reduction Factor (if applicable).

The Percentage can either be a fixed Percentage for all members or a
Member Specific Percentage. To use a fixed Percentage enter the value ie
for 25% enter `25`. To use a Member Specific Percentage, select from the
drop-down list the data item containing the appropriate value. To value
commutation of 25% of the PUP ensure the data item contains the value
25.

**General** Commutation is restricted to avoid commuting the GMP. There
is no allowance for post-retirement increases in calculating this
restriction.

**Cash Data Item** SuperVal does not have the functionality to value an
explicit Cash Commuted Data item. However, as a work around users can
enter the Member Specific Commuted Cash as a data item in the [Cap Cash
Amount](deferreds_basis+datacashcap.md) below. They should then enter
either a Percentage or a Multiple here. The Percentage or the Multiple
entered should be sufficiently large so that the data item entered in
the Cap Cash Amount will bite for all members.
