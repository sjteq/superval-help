# Accrual of Service Related Accrual

This field is only applied when using the [Service Related Accrual
Table](actives_basis+sratab.md) field on the Slices Tab. Select from
the drop-down list whether to use Uniform or Non-Uniform accrual.

When ‘Uniform’ is selected the benefits are spread proportionately
between past and future service assuming that accrual in each year is at
the average rate of accrual for the member over their total service. For
example, in certain schemes where there is ‘double accrual’ after 20
years, the past service liability will take account of any future period
with double accrual that may apply to their benefits even if they have
not yet reached the point where double accrual begins. The user will
then have the option to Cap the accrued service using [Uniform Cap
Accrual](actives_basis+capaccrual.md).

When `Non-Uniform` is selected the benefits are not spread
proportionately. Under this option, using the example above, the past
service liability only takes account of any double accrual that has
actually taken place up to the valuation date



Consider a scheme where the accrual is 1/60<sup>th</sup> up to 20 years
and 1/30<sup>th</sup> thereafter. The only decrement is retirement which
occurs after 30 years of actual service. In SuperVal, the accrual rate
will be set to 1/60<sup>th</sup> and the Service Related Accrual Table
will contain the number of 60<sup>ths</sup> the member receives at each
duration. At 30 years this will be 40.

A member currently has 10 years of service.

-   Under uniform accrual their past service will be $\frac{10}{30} \times 40 = 13.3$
years or $\frac{13.33}{40} = 33\%$ of total liability
-   Under non-uniform accrual their past service will be 10 years or 
    $\frac{10}{40} = 25\%$ of total liability

Consider the same scheme but with a member who has 25 years of service.

-   Under uniform accrual their past service will be 
	$\frac{25}{30} \times 40 = 33.3$ years or 
	$\frac{33.33}{40} = \83%$ of total liability
-   Under non-uniform accrual their past service will be 
	$(20 + 2 \times 5) = 30$ years or $\frac{30}{40} = 75\%$ of total liability
