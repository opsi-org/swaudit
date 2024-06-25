# Changelog swaudit

## [4.3.1.0-1] - 2024-06-25

### Fixed

- Remove keyfinder (Jan Schneider <j.schneider@uib.de>)

## [4.3.0.1-1] - 2024-05-25

### Fixed

- Fix for appx and msix packages (detlef oertel <d.oertel@uib.de>)

## [4.3.0.0-1] - 2024-05-07

### Changed

- Added appx and msix packages via powershell (detlef oertel <d.oertel@uib.de>)
- new property win_get_appx_data bool (default=false)If true get the Appx and Msix Data but this takes some minutes (detlef oertel <d.oertel@uib.de>)

## [4.2.0.1-2] - 2023-10-24

### Changed

- Added "windowsmode" ProductProperty to control behavior of opsi-script window (Nils Doerrer <n.doerrer@uib.de>)

## [4.2.0.1-1] - 2023-05-20

### Changed

- give "windows 11" as name if it is windows 11 (detlef oertel <d.oertel@uib.de>)
- opsi-script >= 4.12.4.35 needed (for getMsVersionName) (detlef oertel <d.oertel@uib.de>)
- default for property win10subversion is now: win10osbuild (detlef oertel <d.oertel@uib.de>)
- code cleanup (detlef oertel <d.oertel@uib.de>)

## [4.2.0.0-1] - 2021-10-19

### Fixed

- Find correct Win10 Release IDs (e.g. 20H2) ; fixes #4692 (detlef oertel <d.oertel@uib.de>)

## [4.1.0.5-1] - 2021-02-15

### Changed

- avoid invalid json objects (detlef oertel <d.oertel@uib.de>)
- macos: check if Info.plist is text file (detlef oertel <d.oertel@uib.de>)
- macos: search for Info.plist only in /Applications/*/Info.plist (detlef oertel <d.oertel@uib.de>)

## [4.1.0.4-1] - 2020-06-10

### Changed

- mark linux and mac software in subversion data field (detlef oertel <d.oertel@uib.de>)
- code cleanup and beautify (detlef oertel <d.oertel@uib.de>)
- avoid warnings at debian (detlef oertel <d.oertel@uib.de>)

## [4.1.0.3-1] - 2020-03-17

### Fixed

- reintegrate fixes from 4.1.0.0-3 (detlef oertel <d.oertel@uib.de>)
- reintegrate fixes from 4.1.0.0-2 (detlef oertel <d.oertel@uib.de>)

## [4.1.0.2-1] - 2020-02-12

### Changed

- macos integration extended (detlef oertel <d.oertel@uib.de>)
- code redesign with defined functions (detlef oertel <d.oertel@uib.de>)

### Fixed

- shellInAnIcon_deb: no rc state pakages: fixes: #4402 (detlef oertel <d.oertel@uib.de>)

## [4.1.0.1-1] - 2020-02-06

### Changed

- macos integration (detlef oertel <d.oertel@uib.de>)

## [4.1.0.0-3] - 2019-04-01

### Changed

- new product property win10subversionvalues: ["win10osbuild", "hklmproductid"]default: ["hklmproductid"]hklmproductid showrsa  begin of HKLM\Software\Mscrosoft\Windows NT\CurrentVersion] ProductId (for example 00330-71317)win10osbuild shows OS Build as found on https://docs.microsoft.com/en-us/windows/windows-10/release-information on on Win10 , Win 2016 , Win2019 from "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion", "CurrentBuild" and "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion", "UBR" (bardo wolf <b.wolf@uib.de>)

## [4.1.0.0-2] - 2018-07-02

### Fixed

- try to fix #2018062810000028 wmic fails with "Beschreibung = Ausnahmefehler aufgetreten." but powershell seems to work (bardo wolf <b.wolf@uib.de>)

## [4.1.0.0-1] - 2018-04-19

### Changed

- new property include_win_hotfixes (default=true) (detlef oertel <d.oertel@uib.de>)
- if wmic call for hotfixes failed retry with powershell (detlef oertel <d.oertel@uib.de>)

## [4.0.7.6-2] - 2017-09-06

### Changed

- use of property 'max loglevel' modified (detlef oertel <d.oertel@uib.de>)

## [4.0.7.6-1] - 2017-09-06

### Fixed

- fix version in Linux swaudit (detlef oertel <d.oertel@uib.de>)

## [4.0.7.5-1] - 2017-09-01

### Changed

- integrate Linux swaudit (detlef oertel <d.oertel@uib.de>)
- append win10 ReleaseId to displayversion of windows (detlef oertel <d.oertel@uib.de>)
- onyly one Logline per product (detlef oertel <d.oertel@uib.de>)
- Use in service mode %opsiserviceUser% as $clientId$ (detlef oertel <d.oertel@uib.de>)
- windows 10 version is now 10 (not 6.3 (from registry)) (detlef oertel <d.oertel@uib.de>)

## [4.0.7.4-2] - 2017-01-25

### Changed

- max loglevel property added to create the option of limiting log file size (rupert roeder <r.roeder@uib.de>)

## [4.0.7.4-1] - 2016-12-08

### Fixed

- fix problems with quatations in uninstall key ( #2481) (detlef oertel <d.oertel@uib.de>)

## [4.0.7.3-1] - 2016-10-12

### Changed

- trim entries to DB field length (detlef oertel <d.oertel@uib.de>)

## [4.0.7.2-1] - 2016-10-12

### Fixed

- fix for readfromfile (detlef oertel <d.oertel@uib.de>)
- mask single quotes by double single quotes before sending (detlef oertel <d.oertel@uib.de>)

## [4.0.7.1-1] - 2016-10-05

### Changed

- code cleanup (detlef oertel <d.oertel@uib.de>)
- complete redesign of webservice connection (detlef oertel <d.oertel@uib.de>)
- requires opsi-scrip 4.11.6 (detlef oertel <d.oertel@uib.de>)

### Removed

- removed opsi3 support (detlef oertel <d.oertel@uib.de>)
- cleanup removed property extended_search (detlef oertel <d.oertel@uib.de>)
- removed win2k support (detlef oertel <d.oertel@uib.de>)
- usekeyfinder now has default off (detlef oertel <d.oertel@uib.de>)
- new property debug_send: Send data using one serviceall per object (detlef oertel <d.oertel@uib.de>)

## [4.0.6-3] - 2015-06-29

### Changed

- use new opsi-script functions if possible:isValidUtf8String(str:string) : boolean;getFixedUtf8String(str:string) : string; (detlef oertel <d.oertel@uib.de>)

## [4.0.6-2] - 2015-11-25

### Removed

- removed property extended_search (was working on xp only) (bardo wolf <b.wolf@uib.de>)

## [4.0.6-1] - 2015-10-29

### Changed

- back to /saveini instead of savecsv "%SCRIPTPATH%\keyfinder\keyfinder.exe" /close /saveini "c:\opsi.org\tmp\" /file "swaudit_keys.ini (bardo wolf <b.wolf@uib.de>)

## [4.0.5-3] - 2015-06-29

### Fixed

- Script fixes for win10 (detlef oertel <d.oertel@uib.de>)
- Go back to old but open source keyfinder (detlef oertel <d.oertel@uib.de>)

## [4.0.6-1] - 2015-04-07

### Changed

- Updated keyfinder. (Niko Wenselowski <n.wenselowski@uib.de>)

## [4.0.5-2] - 2014-11-12

### Fixed

- Fix handling of keys containing quotation marks (detlef oertel <d.oertel@uib.de>)

## [4.0.5-1] - 2014-08-01

### Fixed

- Fix writing to long entries in sub_create_hash4 by adding to all string values something like "name="+strPart($name$,"1","99") (detlef oertel <d.oertel@uib.de>)
- codecleanup (detlef oertel <d.oertel@uib.de>)
- changelog to control file (detlef oertel <d.oertel@uib.de>)

## [4.0.2-3] - 2013-08-05

### Fixed

- Fix duplicate entry: truncating all parts of the primary key to their max length in the DB: "name="+strPart($name$,"1","99") (detlef oertel <d.oertel@uib.de>)
- ScriptErrorMessages = off (detlef oertel <d.oertel@uib.de>)

## [4.0.2-2] - 2012-12-06

### Changed

- switch to ekeyfinder (https://sourceforge.net/projects/ekeyfinder/) (detlef oertel <d.oertel@uib.de>)

## [4.0.2-1] - 2012-08-10

### Changed

- code cleanup (detlef oertel <d.oertel@uib.de>)
- remove all opsi 3 stuff (detlef oertel <d.oertel@uib.de>)
- use opsi-winst 4.11.3 methods (detlef oertel <d.oertel@uib.de>)
- extended search off by default (no data at NT6) (detlef oertel <d.oertel@uib.de>)
- replace delete by del (detlef oertel <d.oertel@uib.de>)
- replace c:\tmp by c:\opsi.org\tmp (detlef oertel <d.oertel@uib.de>)

## [4.0-15] - 2012-05-11

### Changed

- new property: readfromfile to switch off audit and use the filebuffer files insteadONLY DEBUG - do not use if you are not shure what you doing! (Do not make a audit but read values from c:\tmp and send them) (detlef oertel <d.oertel@uib.de>)

## [4.0-14] - 2012-04-26

### Fixed

- workaround for bug#354 (set version to '' if zero) deleted becaus it is fixed (detlef oertel <d.oertel@uib.de>)

## [4.0-13] - 2012-03-15

### Changed

- set version to '' if zero - workaround for bug#354 (detlef oertel <d.oertel@uib.de>)

## [4.0-12] - 2011-11-29

### Changed

- new property: usekeyfinder to switch off keyfinder call (detlef oertel <d.oertel@uib.de>)

## [4.0-11] - 2011-11-04

### Changed

- ' are now escaped (rupert roeder <r.roeder@uib.de>)

## [4.0-10] - 2011-11-04

### Changed

- bugfix, displayname was not newly read (rupert roeder <r.roeder@uib.de>)

## [4.0-9] - 2011-11-03

### Changed

- if displayname contains a ' char the part of the name starting with ' is eliminated (rupert roeder <r.roeder@uib.de>)

## [4.0-8] - 2011-10-18

### Changed

- internal switch for readfromfile (only for debugging: send file data over service) (detlef oertel <d.oertel@uib.de>)
- new property usefilebuffer (dirty workaround for strange not handled control chars) (detlef oertel <d.oertel@uib.de>)

## [4.0-7] - 2011-01-21

### Fixed

- retrun failed if write back to server fails workaoround for #219; fixes #218 (detlef oertel <d.oertel@uib.de>)

## [4.0-6] - 2010-11-15

### Changed

- possibility to write results to file (detlef oertel <d.oertel@uib.de>)
- sub_get_windows_info works now also at win2k (detlef oertel <d.oertel@uib.de>)

## [4.0-5] - 2010-09-27

### Changed

- Using ms product id for subVersion field (Jan Schneider <j.schneider@uib.de>)

## [4.0-4] - 2010-09-15

### Changed

- added property to control use of slowinfocache (detlef oertel <d.oertel@uib.de>)

## [4.0-3] - 2010-08-31

### Changed

- integrating wmic call for nt6 hotfixes (detlef oertel <d.oertel@uib.de>)
- LogLevel optimized (detlef oertel <d.oertel@uib.de>)

## [4.0-2] - 2010-08-24

### Changed

- bugfix: for opsi 3: ending '}' was set before sub_get_windows_info (detlef oertel <d.oertel@uib.de>)
- bugfix: for opsi 3: integrated convert2json (detlef oertel <d.oertel@uib.de>)

### Removed

- bugfix: for opsi 3: double "" removed (detlef oertel <d.oertel@uib.de>)
- bugfix: for opsi 3: Opsiservicecall with '' instead of "" (detlef oertel <d.oertel@uib.de>)
- bugfix: for opsi 3: no mor recompose of uninstallstring (detlef oertel <d.oertel@uib.de>)
- 'last used' and 'usage frequency' removed referring to data privacy compliance (detlef oertel <d.oertel@uib.de>)
- added: support for win2k (without reg command) (detlef oertel <d.oertel@uib.de>)

### Fixed

- bugfix: ends with fatalError if service call fails, fixes #81 (detlef oertel <d.oertel@uib.de>)

## [4.0-1] - 2010-05-11

### Changed

- using winst only (swaudit4.ins) (detlef oertel <d.oertel@uib.de>)

## [1.3-4] - 2009-09-04

### Changed

- Added log file (Jan Schneider <j.schneider@uib.de>)

## [1.3-4] - 2009-09-04

### Changed

- Added log file (Jan Schneider <j.schneider@uib.de>)

## [1.3-3] - 2009-08-04

### Changed

- Compiled using py2exe (Jan Schneider <j.schneider@uib.de>)

## [1.3-2] - 2009-05-17

### Changed

- exe-Version mit eingeschaltetem DEBUG (Erol Ueluekmen <e.ueluekmen@uib.de>)

## [1.3-1] - 2009-04-09

### Changed

- exe-Version (Erol Ueluekmen <e.ueluekmen@uib.de>)

## [1.2.3-3] - 2009-03-16

### Changed

- get installed os (Jan Schneider <j.schneider@uib.de>)
- some bugfixes in charset de/encoding (Jan Schneider <j.schneider@uib.de>)
