# Financial Globals

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
