# V9Migration: Parms



## Table of Migration Default Names

You can use a previously defined set of Migration Names for the Global
Parameters contained in the Basis Files being migrated. Select from the
drop-down list the relevant set to use.

To define a new table of Migration Names, click the Add/Edit Default
Names button.

## Add/Edit Default Names

Clicking the _Add/Edit Default Names_ button allows you to create or edit
a set of Migration Names. The text entered in the Migration Names will
be used as the Global Variable Name for all of the Global Parameters
migrated of that type.

If a set of Migration Names does not exist, then you will be taken
directly to the Migration Names Table where you can enter the default
name to be used for each variable.

If a single set of Migration Names already exists, then you will be
taken directly to this set to enable changes to be made.

If more than one set of Migration Names already exist, then you will be
taken to the Parameter Selection Box to choose which set to open.

## Store Financial Globals under Description

The user can create additional Financial Global Sets on subsequent
migrations, by changing the description. Within the Financial
Assumptions area of SuperVal the user will be able to select which set
of financials to use.

## Match Existing Financial Globals where matching Financial Assumptions found

## Membership Groups (ie Actives, Deferreds and Pensioners kept separate)

## Field Types (eg Pre and Post Retirement Interest Rates kept separate)

The user has the choice on how the Financial Assumptions are migrated.

**Match Existing Financial Globals where matching Financial Assumptions
Found** - Check this box if you would like the existing Global Financial
Parameters defined in the Financial file to be used where a matching
assumption is found in the basis being migrated. Leave this box
unchecked to create a duplicate Global Financial Parameter. (This may be
appropriate where two different basis files use the same value for a
Global Variable as a coincidence.)

## Differentiate unmatched Global Financial Assumptions by the following

`Membership Groups (ie Actives, Deferreds and Pensioners kept separate)`

: Check this box if different Financial Global Parameters should be created for each Membership Category i.e. actives, deferreds, pensioners. This will create a separate set of pointers for each of the Actives Deferreds and Pensioners; allowing management of the migrated financial assumptions by membership group.

`Field Types (eg Pre and Post Retirement Interest Rates kept separate)`

: Check this box to create separate pointers for Pre and Post Retirement Discount Rates with the same value. Leave the box unchecked if only one interest-rate parameter should be created.

## Actives

## Deferreds

## Pensioners

Check this box if you wish to use existing Global Parameter Sets for
Mortality/Mortality Improvements where these are already defined.

Leave this box unchecked to create a new Global Parameter Set for each
set migrated.

## Back

Clicking on the _Back_ button allows you to return to the previous screen.

## Next

Click the _Next_ button, once you are happy with the selections made, to
move to the next screen.

## Cancel

Clicking on the _Cancel_ button allows you to return to the previous
screen without saving any of your changes.