# Spreading Method For Prospective Element

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
Start Date](actives_basis+ssd.md) to [Spreading Finish
Date](actives_basis+sfd.md). For normal FAS values, Spreading Start
Date should be set to DJF and Spreading Finish Date to LDATE.

The `Projected Unit` option values the full prospective element for
those who exit within the control period only. For those who do not exit
during the control period, only the benefit based on accrued service is
valued. Spreading dates are ignored. For attained age valuations,
SuperVal values the full prospective element for all future exits, i.e.
the control period is infinite.

Not all options are available to all users.
