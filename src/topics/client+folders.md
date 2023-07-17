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
