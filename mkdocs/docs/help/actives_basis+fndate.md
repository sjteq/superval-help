# Service Finish Date/Latest Finish Date

The Service Finish Date for each slice is entered here. Select from the
drop-down list the data item containing the relevant data item. This
will be used as the date when service for this Slice stops accruing
unless a Latest Finish Date is also defined.

The user can define the Latest Finish Date that can be used for a
particular Slice. Enter this date in the following date format
DD/MM/CCYY. SuperVal will then take the earlier of these two dates to
determine when service for this Slice stops accruing.

If valuing future service, the Service Finish Date on Slice 1 will
always be `Leaving Date`. The Latest Finish Date could be used to cease
accrual at a fixed date in the future. If you have no future service
liabilities, please ensure these fields are left blank on Slice 1. The
Latest Finish Date will not be used for future service benefits on Slice
1 when CARE benefits are being valued.

If the Slice is being used to value added years or a fixed pension then
these field can be left blank.

The Latest Finish Date on the [Offset Slice](actives_basis+sliceup.md)
must be specified as this is used to identify the date at which GMPs
stopped accruing, for some Cash Commutation or death in deferment
options.
