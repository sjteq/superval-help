# Commutation Tables



## Calculate Commutation Factors based on Valuation Basis

SuperVal will calculate commutation factors applicable to each
individual member using the valuation basis and the all relevant Basis
Parameters (Guarantee Period, Post Retirement Mortality, Post Retirement
Interest rate and Pension Increases).

## % of Valuation Basis Factor

Users
can define the % of Valuation Basis Factor they want to apply to the
Scheme. To have this field visible the above field `Calculate
Male/Female Commutation Factors based on Valuation Basis` needs to be
ticked. The Valuation Factors produced by SuperVal can be seen in
individual VARPRINTs.

## Main Increase Commutation Table

## Special Increase Commutation Table

## PenInc3 Commutation Table

## PenInc4 Commutation Table

Double click to select the rate table containing the Commutation Factors
ie the amount of cash received for each pound per annum of pension
commuted. Please note that SuperVal assumes exits prior to NRA occur
half-way through the year i.e. 0.5 years, 1.5 years etc after the
valuation date. Exits at NRA occur at the beginning of the year. This
should be reflected in the Commutation Factors entered into the table ie
for ages prior to NRA the factor in the table should be the factor that
would apply at the point of exit.

For example, a factor of 9 at age 65 means that for every pound
surrendered in pension at age 65 the member would receive £9 in cash.

Separate tables can be specified for males and females and for each of
the different pension increase rates (Main, Special, Pension Increase 3
and Pension Increase 4) being used.

Even if cash is payable on top of pension benefits, cash commutation
factors are still required for application of IR Maximum rules.

### Related



-   [Selecting rate tables](selecting_rate_tables.md)

## Decr Help

Rate tables can be selected by any of the following methods:

-   Right-click on the field for a list of appropriate Rate Tables. For
    a field that will accept more than one type of Rate Table (e.g.
    Miscellaneous Tables), the list will be restricted to the current
    Table Type specified in the field – if you wish to see all allowable
    Rate Tables, delete the Table Type from the field before clicking;
    or
-   Double Clicking on the field will produce the Rate Tables form where
    Rate Tables can be viewed (numerically and graphically) and Rate
    Tables can be added or edited. A Rate Table can be selected by
    pressing the Select button or double clicking on the Rate Table
    description in the tree; or
-   the list of allowable Rate Tables can be scrolled through by
    pressing the `<` or `>` keys. The description of the Rate Table to
    the right of the field will change as each new Table is selected.

## Linearly Interpolate Commutation Tables for mid-point Exit values

When checked, the system will linearly interpolate factors for mid year
exits such as early retirements and deaths. For Normal Retirements, the
system will apply no interpolation. If unchecked, the system will use
the factor specified at the age nearest rounded down for mid year exits
as previous versions have done.

## Adjust Commutation Tables by the change in member's expectation of life

Future mortality-improvement assumptions underlying the Technical Provisions can be applied to the tabulated commutation factors in force at the valuation date, to calculate revised commutation factors at the date of exit.

## SaveAs

Click the _Save As_ button to save with a new file name.

## Save

Clicking on the _Save_ button allows you to save the entries.

## Quit

Clicking on the _Quit_ button allows you to exit without saving any of
your changes.

In some of the screens you will be asked to confirm if you want to exit
_Ignoring all changes_. If you click _Yes_, the file will be closed
without saving any changes. If you click _No_ you will be returned to your
original screen.

From the Browser, the _Quit_ button will take you to a graphical display
of the results.