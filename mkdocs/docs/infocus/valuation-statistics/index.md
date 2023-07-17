---
title: Valuation statistics
author: Khiloni Shah
date: March 2019
header-includes: 
- \usepackage[sfdefault]{FiraSans}
- \usepackage{graphicx}
- \usepackage{fancyhdr}
- \pagestyle{fancy}
- \setlength{\footskip}{60pt}
- \fancyfoot[L]{\includegraphics[width=5mm]{../img/superval.png} \textit{SuperVal InFocus}}
- \fancyfoot[R]{\includegraphics[width=20mm]{../img/eps.png}}
- \fancyfoot[C]{\thepage}
- \fancyhead[R]{Valuation statistics}
---

<!-- # Valuation statistics -->


_How the calculations in the Valuation Statistics
are produced as part of the Excel output._

## Weighted averages by number of members

Age by Number of Members

: Age is calculated at the Valuation Date as Age Nearest Year.

	This is the sum of each member’s Age divided by the Number of Members.

Salary by Number of Members

: This is the sum of all members’ Member Contributions Salary at the Valuation Date divided by the Number of Members.

Past Company Service/Scheme Membership by Number of Members

: This calculation is done separately for Member’s Company Service and Member’s Scheme Membership. 

	It is the sum of all members’ service to the
	Valuation Date as defined by the two data items, Date Joined Company and
	Date Joined Scheme, divided by the Number of Members. It will not
	include service from periods defined outside of the data items e.g.
	added years service.

Future Membership Service by Number of Members

: This is the sum of all member’s service from the Valuation Date to the member’s Normal Retirement Date as defined in the Category divided by the Number of Members. It will not include additional service built up after the Valuation Date in the form of Additional Credits.

Total Company Service/Scheme Membership by Number of Members

: This calculation is done separately for Member’s Company Service and Member’s Scheme Membership. 

	It is the sum of all members’ service from
	either Date Joined Company or Date Joined Scheme to the member’s Normal
	Retirement Date as defined in the Category divided by the Number of
	Members. It will not include service from periods defined outside of the
	data items e.g. added years service or additional service built up after
	the Valuation Date in the form of Additional Credits.

Age at Entry to company/Scheme Membership by Number of Members

: This is the sum of the age of all members at either Date Joined Company or Date Joined Scheme divided by the Number of Members.


## Weighted averages by members’ contribution salary

The salary used to determine these average ages is the salary defined
for Member Contributions as at the Valuation Date (“SAL”).

Age by Members’ Contribution Salary

: Age is calculated at the Valuation Date as Age Nearest Year.

	This is the sum of each member’s Age multiplied by SAL divided by the
	sum of SAL.

Past Company Service/Scheme Membership by Members’ Contribution Salary

: This calculation is done separately for Member’s Company Service and Member’s Scheme Membership. 

	It is the sum of all members’ service to the
	Valuation Date as defined by the two data items, Date Joined Company and
	Date Joined Scheme, multiplied by SAL divided by the sum of SAL. It will
	not include service from periods defined outside of the data items e.g.
	added years service.

Future Membership Service by Members’ Contribution Salary

: This is the sum of all member’s service from the Valuation Date to the member’s Normal Retirement Date as defined in the Category multiplied by SAL divided by the sum of SAL. It will not include additional service built up after the Valuation Date in the form of Additional Credits.

Total Company Service/Scheme Membership by Members’ Contribution Salary

: This calculation is done separately for Member’s Company Service and Member’s Scheme Membership. 

	It is the sum of all members’ service from
	either Date Joined Company or Date Joined Scheme to the member’s Normal
	Retirement Date as defined in the Category multiplied by SAL divided by
	the sum of SAL. It will not include service from periods defined outside
	of the data items e.g. added years service or additional service built
	up after the Valuation Date in the form of Additional Credits.

Age at Entry to Company/Scheme Membership by Members’ Contribution Salary

: This is the sum of the age of all members at either Date Joined Company or Date Joined Scheme multiplied by SAL divided by the sum of SAL.


## Weighted averages by company contribution salary

The salary used to determine these average ages is the salary defined
for Company Contributions as at the Valuation Date (`SAL`).

Age by Company Contribution Salary

: Age is calculated at the Valuation Date as Age Nearest Year.

	This is the sum of each member’s Age multiplied by SAL divided by the sum of SAL.

Past Company Service/Scheme Membership by Company Contribution Salary

: This calculation is done separately for Member’s Company Service and Member’s Scheme Membership. 

	It is the sum of all members’ service to the
	Valuation Date as defined by the two data items (Date Joined Company and
	Date Joined Scheme) multiplied by SAL divided by the sum of SAL. It will
	not include service from periods defined outside of the data items e.g.
	added years service.

Future Membership Service by Company Contribution Salary

: This is the sum of all member’s service from the Valuation Date to the member’s Normal Retirement Date as defined in the Category multiplied by SAL divided by the sum of SAL. It will not include additional service built up after the Valuation Date in the form of Additional Credits.

Total Company Service/Scheme Membership by Company Contribution Salary

: This calculation is done separately for Member’s Company Service and Member’s Scheme Membership. 

	It is the sum of all members’ service from
	either Date Joined Company or Date Joined Scheme to the member’s Normal
	Retirement Date as defined in the Category multiplied by SAL divided by
	the sum of SAL. It will not include service from periods defined outside
	of the data items e.g. added years service or additional service built
	up after the Valuation Date in the form of Additional Credits.

Age at Entry to Company/Scheme Membership by Company Contribution Salary

: This is the sum of the age of all members at either Date Joined Company or Date Joined Scheme multiplied by SAL divided by the sum of SAL.


## Weighted average age by past service liability

Age by Past Service Liability

: Age is calculated at the Valuation Date as Age Nearest Year.

	The Past Service Liability (PSL) is calculated within SuperVal.

	This is the sum of each member’s Age multiplied by PSL divided by the
	sum of PSL.


## PV 1% of salaries

This statistic is shown for 60 years after the Valuation Date.

:fontawesome-solid-hand-point-right:
[Calculation of PV 1% Salaries](../calculation-of-pv-1pct-salaries/index.md)


## Weighted average future working lifetime

The Present Value of 1% of Salaries is also displayed for four different
periods which are based on an estimate of the Average Remaining Future
Working Lifetime of the members. These periods are calculated as
follows:

By Number of Members

: The sum of the Future Service after the Valuation Date multiplied by the probability of exit (at each future exit point) weighted by the Number of Members.

By Members’ Contribution Salary

: The sum of the Future Service after the Valuation Date multiplied by the probability of exit (at each future exit point) weighted by the Members’ Contribution Salary at the Valuation Date. No allowance is made for increases to Salary after the Valuation Date.

By Company Contribution Salary

: The sum of the Future Service after the Valuation Date multiplied by the probability of exit (at each future exit point) weighted by the Company Contribution Salary at the Valuation Date. No allowance is made for increases to Salary after the Valuation Date.

By Projected Salary

: This is the sum of the PV 1% of Salaries over all future years divided by the PV 1% of Salary in the year after the Valuation Date.

## Company normal cost as % of all members’ salaries

For the Projected Unit Credit method of valuation, the cost of benefits
accruing for all members in each future projection year is displayed as
a percentage of the PV 1% of Salary in that projection year.
