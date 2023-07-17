# Client: Files



## Scheme Name

Enter the Scheme Name.

The Scheme Name will appear in the header of all output created for this
Scheme. If different sets of calculations are produced in different
folders i.e. current and previous valuations or transfers out then a
description of the purposes of the calculations could also be included.

## Yield Curve Files Folder

## Output Files  Folder

## Consolidation Results File Folder

## Mortality Improvement Files Folder

SuperVal allows different folder paths to be specified for different
purposes and therefore allows valuations to be processed more
efficiently.

Select *File+Open Scheme Folders* on the main menu bar to view the
current list of the Folder pathnames.

A list of the Folders used by SuperVal and their purpose is as follows:

folder | description
-------|-------------
Input | Contains all member data and parameter files.
Yield Curve | Contains yield curves; if blank defaults to Input Folder
Output | All valuation results output files (including the consolidated output) will be written to the folder path specified here.
Consolidation | This folder is where the results database will be written (SVResultsDB)
Mortality Improvement | Contain mortality improvement tables; default is library folder

The above folders contain all the files used for a particular Scheme
Valuation. Note that it is not necessary to specify these as different
folder paths. Input, Yield Curve, Output and Consolidation can all be the same folder
path if preferred. If Mortality Improvement is at the system level though, it must be on the same drive as the library folder.

Having the Consolidation as a different folder will enable different
users to process separately actives, deferreds and pensioners while
still being able to consolidate all Scheme membership. To do this all
users for a particular scheme should specify the same folder path for
the Consolidation folder.

Double click to select the Folder locations.

## S21 Migration Required

Check this box if you are migrating the input files from a previous
version of SuperVal.

## Superval/21 Migration Folder

The Folder containing the SuperVal system files for the Scheme
(`CLIENT.sf`, `DEFAULT.sf`, `BASIS.sf` and named basis files) that are to be
migrated.

## Mortality Improvement Files

Specify where the Mortality Improvement csv files are stored.
i.e. whether stored at a scheme level or at a system level.

## Scheme Level Parameter File

Specify the name of the Scheme Level Parameters File.

If any Scheme Level Parameters File(s) already exist in the Scheme
Folder, they will be displayed in the list. If there are more than one,
you must select the one you wish to use for this session.

If there are no Scheme Level Parameters Files in the Scheme Folder, the
list displayed will be blank. In this case, you must type in the name of
the Scheme Level Parameter File. It is recommended to specify a name
that describes the Scheme (and/or the purpose of the calculations if
there are more than one Folder for the Scheme) so that the file will be
easily recognisable at a later date.

Note that any parameters in other Scheme Level Parameter File(s) in the
Scheme Folder will not be available unless you log-off and commence a
new session in the Scheme Folder selecting that other Scheme Level
Parameter File.

One Scheme Level Parameter File per Scheme Folder is the recommended
configuration.

## Scheme Basis Parameter File

Article missing from client+basisfile.md

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