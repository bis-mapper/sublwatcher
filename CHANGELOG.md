## 1.0.2(BETA)
  - Growl notification on save
  - Bug fix with error routine not defined
  - Removed config param <appbuilds>
  - Lowered BASHEXEC_ timeout
  - Fixed bug with error message in BASHEXEC_
  - When exporting WARN if drawer description is blank
  - Skip drawers with DUMPS in the description
  - Change growl to use DEFINE instead of registered run.

## 1.0.0(BETA)
  - Allows DIFFs across different sites
  - No longer crashes when doing DIFF on non-existent file
  - Warns whether a report is locked instead of just rep over it
  - BDT will re-open the defines report
  - Growl Warning when updates outside of report boundaries have been discarded
  - Allows replacing of Report 0 if needed
  - Added current USER$ to screen
  - Added site letter to Update Control warning
  - Added option to do DIFF on Update Control Warning dialog
  - Allows a report that is saved to be created if it does not currently exist
  - Displays warning when trying to open a report that doesn't exist
  - Changes are saved and retrieved from site folder instead of root, allowing instance on multiple sites without saving over the wrong site

## 0.0.12
  - bug fixes

## 0.0.11

Features:

  - add support for IBLD within Sublime
  - add ability to REG run within Sublime
  - add new drawer(I) fore error dumps
  - modified error routine to capture dumps and send email in-house

Documentation:

  - changed Growl to be registered run instead of using DEFINE_

