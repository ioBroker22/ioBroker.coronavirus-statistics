# Older changes
## 0.8.2 (2021-08-17)
* (DutchmanNL & jlssmt) Small code improvements to prepare stable release 

## 0.8.1 (2021-08-16)
* (DutchmanNL) added definitions for total_boosters

## 0.8.0 (2021-08-12)
* (jlssmt) Added vaccination data for all countries
* (DutchmanNL) added definitions for vaccination states
* (DutchmanNL) Folder structure optimized with devices and channels
* (DutchmanNL) Code improvement to handle state deletion more efficient
* (DutchmanNL) Changeover to validated API for German vaccination data of Bundesländer
* (DutchmanNL) Ensure (country) folder(s) including all states are removed if not selected

## 0.7.2 (2021-06-30)
* (jlssmt) New vaccination data source for German (our world in data)

## 0.7.1 (2021-06-30)
* (DutchmanNL) Bugfix: Vaccination data for Germany

## 0.7.0 (2021-06-28)
* (DutchmanNL) round Impfquote to 2 digits
* (DutchmanNL) Bugfix: Solved last_update is invalid warn message
* (DutchmanNL) Bugfix: State attribute definition missing for + undefined
* (DutchmanNL) Bugfix: Solved cannot read property 'Erstimpfung' of undefined
* (DutchmanNL) Bugfix: State value to set for "xxx.BL" has to be type "number" but received type "string", solves [#237](https://github.com/DrozmotiX/ioBroker.coronavirus-statistics/issues/237)
* (DutchmanNL) Bugfix: State value to set for "xxx.Tests*" has to be type "string" but received type "number", solves [#237](https://github.com/DrozmotiX/ioBroker.coronavirus-statistics/issues/237)
* (DutchmanNL/jlssmt) Bugfix: Vaccination data for Germany, several states missing in new API and will not be updated anymore !

## 0.6.9 (2021-03-22)

* (lembnau) Adapter issues with vaccination data from Germany solved

## 0.6.8 (2021-01-27)
* (DutchmanNL) Bugfix : Germany vaccination data, source changed code updated
* (DutchmanNL) Removed states (not provided by RKI anymore)
  * Impfungen pro 1.000 Einwohner
  * Indikation nach Alter 
  * Berufliche Indikation
  * Medizinische Indikation
  * Pflegeheim-bewohnerIn
* (DutchmanNL) New states (provided by RKI)
  * Differenz zum Vortag 
  * Gesamtzahl bisher verabreichter Impfstoffdosen
  * Gesamtzahl kumulativ BioNTech
  * Gesamtzahl kumulativ Moderna
  * Impf-quote
  * Zweit Impfungen kumulativ
  * Zweit Impfungen Differenz zum Vortag

## 0.6.7 (2021-01-04) Improve handling of vaccination data for germany
* (DutchmanNL) Added Impfungen pro 1.000 Einwohner
* (DutchmanNL) Bugfix : Proper error handling if excel data cannot be retrieved

## 0.6.6 (2021-01-03)
* (DutchmanNL) Bugfix : Wrong channel creation of _Impfungen
* (DutchmanNL) BugfixWindows :Error: ENOENT: no such file or directory, open 'C:\opt\iobroker\iobroker-data\files\Impfquotenmonitoring.xlsx'

## 0.6.5 (2021-01-02)
* (DutchmanNL) implement Vaccination data for Germany, thank you @winnyschuster for
[RKI-Impfquotenmonitoring Deutschland](https://forum.iobroker.net/topic/40394/skript-rki-impfquotenmonitoring-deutschland-incl-b-länder/3)

## 0.6.4 (2020-12-29)
* (DutchmanNL) change API from V2 to V3
* (DutchmanNL) Add Last_Updated for city's/counties

## 0.6.3 (2020-11-04)
* (DutchmanNL) Bugfix : Error warnings to wrong type in states
* (DutchmanNL) Bugfix : Error values.features is not iterable solved

## 0.6.2 (2020-11-02)
* (stan23) 
add "Cases per 100k" in total & during the last 7 days for Germany's Bundesländer

## 0.6.1 (2020-09-25)
* (stan23) Added cases per 100k during the last 7 days for Germany

## 0.6.0 (2020-08-28)
* (DutchmanNL) Replaced module request with axios
* (DutchmanNL) Bugfix : Proper error handling of failing API calls (if api not reachable)
* (Kampfratte) Bugfix : API-Abfrage geändert

## 0.5.7 (2020-04-17) Continent state attribute information added and warn messages reduced
* (DutchmanNL) Bugfix : Add continent state attribute definition
* (DutchmanNL) Bugfix : Reduce warn messages if error occurs to 1 per message

## 0.5.6 (2020-04-17) Bugfix : API changed
* (Kampfratte) Bugfix : API changed

## 0.5.5 (2020-04-07) Bugfixes, see changelog for details
* (DutchmanNL) Bugfix : Remove test-states
* (DutchmanNL) Bugfix : Selected items not shown in tables
* (DutchmanNL) Bugfix : Remove incorrect countryInfo state
* (Scrounger)  Bugfix : Timestamp for continents calculation
* (Scrounger)  Bugfix : Replace " , " in a country name causing errors
* (DutchmanNL) Bugfix : Saint Pierre Miquelon (iso2: null, iso3: null) not found in lib!
* (DutchmanNL) Implemented Total number of COVID-19 tests taken globally.  
 It reflects the Total Tests' column in the table at https://www.worldometers.info/coronavirus/.

## 0.5.1 (2020-03-31) BugFix : State attribute definition missing for + affectedCountries
* (DutchmanNL) BugFix : State attribute definition missing for + affectedCountries
* (DutchmanNL) BugFix : Ensure name changes are propagated

## 0.5.0 (2020-03-31) For Germany : federal states, counties and cities added
* (DutchmanNL) Update production release from 0.4.0 to 0.5.0
* (DutchmanNL) BugFix : Do not write objects unneeded

## 0.4.9 Fixed issues in country names, added counties and cities for germany
* (DutchmanNL  & AlCalzone) Code optimizations 
* (DutchmanNL) Cities for germany added
* (DutchmanNL) counties for germany added
* (DutchmanNL) Hiding tables if "all" is selected
* (DutchmanNL) Hiding unused tables in advanced settings
* (Kampfratte) BugFix : Country top 5
* (GermanBluefox) BugFix : hidden numbers
* (DutchmanNL) BugFix : Several translations
* (DutchmanNL) BugFix : Issues with integration testing
* (Scrounger)  Bugfix : Country names by ISO format (could result in new data points!)
* (DutchmanNL) BugFix : Deletion of unselected federal states and counties (Germany)
* (DutchmanNL) BugFix : Button only respond when clicking on lable (not all browser)
* (DutchmanNL) BugFix : Ensure incorrect created states for "countryInfo" are removed

## 0.4.5 Countries for Germany added
* (DutchmanNL) Countries for Germany added
* (DutchmanNL) added selection for federal states and country's
* (DutchmanNL) BugFix : State attribute definition missing for + deathsPerOneMillion

## 0.4.2 Federal States for Germany implemented
* (DutchmanNL) Configuration redesigned, moved options to "Advanced Settings" tab
* (DutchmanNL) Federal States for Germany implemented, thanks to : https://npgeo-corona-npgeo-de.hub.arcgis.com/ 

## 0.4.0 Data-points added for Top 5 of countries with most cases
* (KLVN) BugFix : German (and some other) translations corrected
* (DutchmanNL) Add gulp i18n translation structure


## 0.3.5 Data-points added for Top 5 of countries with most cases
* (DutchmanNL) Data-points added for Top 5 of countries with most cases
* (DutchmanNL) BugFix : Flag datapoints are not deleted

## 0.3.4 Add button to read "All Countrys"
* (DutchmanNL) Add button to read "All Countrys"
* (DutchmanNL) Add state for link to flag for each country on github
* (DutchmanNL) BugFix : State attribute definition missing for + countryInfo
* (DutchmanNL) BugFix : Turks_and_Caicos not found in lib! Must be added to the country name translator.

## 0.3.3 Improved configuration page
* (DutchmanNL) Improved configuration page
* (DutchmanNL) Make country list in configuration variable	
* (DutchmanNL) Implement choice if non-selected countrys should be deleted from states (if already there, default No!) 

## 0.3.1
* (DutchmanNL) Enable configuration

## 0.3.0 (2020-03-22)
* (GermanBluefox) The number of data points was reduced by selection of countries
 
## 0.2.5 
* (Scrounger) Bugfix : Cabo_Verde not found in lib! Must be added to the country name translator

## 0.2.4
* (Scrounger) Grouping by continents implemented

## 0.2.3
* (DutchmanNL) Error message for new attribute solved

## 0.2.2
* (GermanBluefox) fixed widget countries

## 0.2.1
* (DutchmanNL) Fixed error "State attribute definition missing"
* (DutchmanNL) Moved "_Laste_Update" to updated within global_totals tree
* (GermanBluefox) fix logo size

## 0.2.0 Code optimized & released
* (DutchmanNL) Stable release
* (DutchmanNL) Added retry if API does not provide correct information
* (DutchmanNL) Added last time stamp of data collection
* (AlCalzone) Code optimized

## 0.1.6 Adapter renamed
* (@DutchmanNL) Adapter renamed

## 0.1.2 Widgets added & code improvements
* (DutchmanNL) code improvements
* (GermanBluefox) add widgets

## 0.1.0
* (DutchmanNL) initial release

