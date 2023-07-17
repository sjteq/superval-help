---
title: Equalisation of Retirement Ages
author: Khiloni Shah
date: March 2019
header-includes:
---

# Equalisation of Retirement Ages


This article covers the Equalisation of Retirement Ages in SuperVal for
the Actives Module.

Where members have different retirement ages in respect of different
periods of service, as a result of equalisation, the user may need to
allow for this when valuing benefits. This article provides some
suggested approaches.

!!! info "Version"

    This article is based on Version 9.20 of SuperVal.
    Any screenshots included from earlier versions of SuperVal are not materially different from those in V9.20.


## Worked example

Suppose a scheme equalised retirement ages for service from
1st January 1993 at 65 for males and females. Retirement ages
were 65 for males and 60 for females prior to this date.

The NRAs for different periods of service are as follows:

    For Service                             NRA (M/F)
    --------------------------------------------------
    up to 17 May 1990                         65/60
    between 17 May 1990 and 1 January 1993    60/60
    from 1 January 1993                       65/65

There are two methods of dealing with this in SuperVal, shown as Method
A and Method B below:

### Method A

This method is used where there is an early retirement decrement
assumption in the valuation basis. It makes use of two sets of early
retirement reduction factors.

### Method B

This method is simpler and involves loading the benefit from a slice by a factor to approximate the higher value.

### Slice structure

The slice structure will be the same for both methods as follows:

Slice 4

    Service Start Date   | DJF
    Not Before Date      |
    Service Finish Date  | VDATE
    Not After Date       | 17051990


Slice 3

    Service Start Date   | DJF
    Not Before Date      | 17051990
    Service Finish Date  | VDATE
    Not After Date       | 01011993


Slice 2

    Service Start Date   | DJF
    Not Before Date      | 01011993
    Service Finish Date  | VDATE
    Not After Date       |


Slice 1

    Service Start Date   | VDATE
    Not Before Date      |
    Service Finish Date  | LDATE
    Not After Date       |



### Further complications

The above slice structure ignores complications for changes in pension-increase rate and any application of an Underpin. If your scheme has
these scenarios then you will need to increase the number of slices as
appropriate.

For example, if the scheme applied LPI 5% on pensions accruing post
5/4/1997 and 3% for pensions accruing pre 6/4/1997 then the slice
structure would be:

Slice 5

: (as for previous Slice 4)

Slice 4

: (as for previous Slice 3)

Slice 3

    Service Start Date   | DJF
    Not Before Date      | 01011993
    Service Finish Date  | VDATE
    Not After Date       | 06041997


Slice 2

    Service Start Date   | DJF
    Not Before Date      | 05041997
    Service Finish Date  | VDATE
    Not After Date       |  

Slice 1

: (as for previous Slice 1)

Slices 1 and 2 apply the LPI 5% pension increase rate, and Slices 3 to
5 apply the 3% pension increate rate.


!!! tip "Rounding override"

    Because periods of service are being split around dates, you need to be careful as to the (service) _Rounding Override_ on the slices.
    Rounding down by months or even years could mean that the total service being allowed for is less than is required.

    To get round this you could round up, or even use days (`DN`)


### Method A

#### Tables and reduction factors

On the _Demographic_ tab enter a non-zero `R` type table for the _Early
Retirement Decrement_.

For example, suppose that an early-retirement decrement rate table is
entered as follows:

    Age     65   64    63    62    61    60    59    58
    -----------------------------------------------------
    Rate    1    0.05  0.05  0.05  0.05  0.05  0.05  0.05

!!! tip "Decrement rates are entered as independent rates and SuperVal derives the dependent rates from these."

Suppose the scheme applies a 4% simple reduction factor for early
retirements. The entries required in tables of the early retirement
reductions factors are as follows:

    Age    65    64    63    62    61    60    59    58
    --------------------------------------------------------
    ERF65  1     0.98  0.94  0.90  0.86  0.82  0.78  0.74
    ERF60  1.50  1.45  1.35  1.25  1.15  1.05  0.98  0.94

ERF65 reflects at NRA of 65 and ERF60 is to reflect an NRA of 60.

In this case it has been assumes that the scheme applies Late Retirement
Factors of 10% pa simple (factors applied to benefit at actual
retirement age).

Note that for ERF65, there is only a reduction of 2% in the first year
early. This is because SuperVal assumes exit benefits payable before NRA
will occur half way through the year. So, for ages below NRA, you need
to enter the factors for age x+ ½. The ERF60 factors show how this
affects the ERFs and LRFs.

(Rate table types for early retirement reduction factors would typically
be `FX` or `HX` type)

The Early Retirement Reduction Factor tables would then be set on the
_Ret Pension_ and _Ret Cash_ tab as follows:


    Field                    | Male Table | Female Table
    -------------------------|------------|-------------
    ERF1 (Revaluation 1 & 3) |   ERF60    |    ERF60
    ERF1 (Revaluation 2)     |            |
    ERF2 (Revaluation 1 & 3) |   ERF65    |    ERF65
    ERF2 (Revaluation 2)     |            |


Consider the Early Retirement Reduction Factors you
want to apply and code the relevant table under ERF1 (Revaluation 1 & 3)
or ERF1 (Revaluation 2). This depends on the parameter set in the
_Revaluation in Deferment_.

!!! tip "Alternative ERFs are to be used for cash-on-top benefits, which can be set on the _Ret Cash_ tab."

#### Withdrawal benefits

If you have a withdrawal decrement, then a loading needs to be applied
to reflect the fact that part of the benefit can be taken at age 60
without a reduction. This is done in the fields “Male/Female Barber
Adjustment to Main/Special/PenInc3/PenInc4” on the _Financial_ tab for
_Deferred Revaluation_.

The loading is necessary because withdrawal benefits will be assumed to
be payable at NRA only. The early-retirement decrement is only applied to
those that stay in service to the early-retirement ages.

Please note that the loading will apply to the part of the withdrawal
benefit arising from the Slice that has _ERF Tables_ set to `1` (for
ERF1).

### Method B

In this method there are no early-retirement decrements or early-retirement reduction factors.

The entire allowance for the Slice of service payable from age 60 is
made via the Pension Adjustment Factor on the Tier of that Benefit Slice
e.g. entering 1.5 in this field will load the pension amount in that
slice by 50%.

Note that if you have withdrawals you will _not_ need to make the
loading adjustment in the fields “Male/Female Barber Adjustment to
Main/Special/PenInc3/PenInc4” on the _Financial_ tab for _Deferred
Revaluation_.
Set these fields to 1.

!!! detail "Early-retirement reduction factor"

    Whatever the factor is in the early-retirement reduction factor table at NRA, it will get applied to the pension amount at NRA.

    This is regardless of the early-retirement decrement at NRA.


## VarPrints

It is always a good idea to check the calculations of the benefits for a
member by running a VarPrint.

The VarPrint will show the benefit amounts, application of early
retirement reduction factor tables, loading adjustments, and annuities.

The sections of the VarPrint that will need consideration here:

Section | Heading | Description
--------|---------|------------
st0<br>(s=slice&nbsp;no,&nbsp;t=tier&nbsp;no.) | Slice Structure | Calculation of the benefit amounts arising in each slice.
990 | Summary of Slice Processing | Will illustrate the amounts of benefit for each particular purpose. In 991 columns A to D will be shown the amounts of benefit to which ERF2 will be applied.
1100 | Early Retirement Pension | Benefit amounts after application of the early retirement reduction factor tables.
2450 | Barber Adjustments to PUPs | Application of the loading adjustment to the withdrawal pension amounts. This is the adjustment outlined in Method A.


Annuities are multiplied by the benefit amounts and their values are
shown in sections 3000 onwards for all the different types of benefit;
retirement, death in service, ill health, leaving service.

###
