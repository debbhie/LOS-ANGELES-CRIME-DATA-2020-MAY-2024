# LOS-ANGELES-CRIME-DATA-2020-MAY-2024

## LOS ANGELES CRIME DATA 2020 - MAY 2024 OVERVIEW
The Los Angeles crime data report provides a comprehensive analysis of crime incident from 2020 -2024. The dataset includes detailed information on the date, location of crimes, the demographic characteristics of victims, the status of cases and other key variables. This report aims to present key performance indicators (KPIS) derived from the dataset to understand crime trends, identidy common crimes and provide insights for potential policy and enforcement improvements.

## DATA SOURCE
The primary data is gotten from data.gov
-[download here](https://catalog.data.gov/dataset/crime-data-from-2020-to-present)

## LANDING PAGE
This expalins each column in the dataset as follows;
* DR_NO: Division of record numbers. This is made up of a 2-digit year, area_id and 5-digits.
* DATE_RPTD: Date and time the incident was reported.
* Date_OCC: Date the incident occured.
* TIME: Time the incident occured, in 24hours military time.
* AREA: The LAPD has 21 community police stations referred to as the geographic area within the department. These geographical areas are subsequentially numbered from 1-21 (API field name).
* AREA_NAME: The 21 geographic areas or patrol divisions are also given a landmark or the surrounding community that it responsible for. For exxample, 77th street, serving neighborhoods in south Los Angeles.
* RPT_DIST_NO: A four digit code that represents a sub-area within a geographical area. All crime records references the "RD" that it occurred in for statistical comparison.
* CRM_CD: Indicates the crime committed (same as crime code1).
* CRM_CD_DESC: Crime code provided.
* MOCODES: Activities associated with the suspect in commission of the crime (modus operandi).
* VICT_AGE: Victims age.
* VICT_SEX: Victims gender (male/female/unknown)
* VICT_DESC: Descent code are as follows; A-other asian, B-bLACK, C-chinese, D-cambodian, F-filipino, G-guamanian, H-hispanic/latin/mexican, I-american indian/alaskan native, J-japanese, K-korean, L-laotian, O-others, P-pacific islander, S-samoan, U-hawaiian, V-vietnamese, W-white, X-unknown, Z-asian indian.
* PREMIS_DESC: The premises where the crime took place.
* WEAPON_USED_CD: The type of weapon used in the crime.
* WEAPON_DESC: Defines the weapon code provided.
* STATUS: Status of the case (IC is the default).
* STATUS_DESC: Defines the status code provided.
* CRM_CD_1: Indicates crime committed. Crime code 1 is the primary and most serious one, Crime code 2,3 and 4 are respectively less serious offenses. Lower crime class number are more serious.
* CRM_CD_2: Contains a code for an additional crime, less serious than crime code 1.
* CRM_DC_3: Contain a code for an additional crime, less serious than crime code 1.
* CRM_CD_4: Contains a code for an additional crime, less serious than crime code 1.
* LOCATION: Street address of crime incident rounded to the nearest hundred block to maintain anonymity.
* CROSS STREET: Cross street of rounded address.
  
## TOOLS
- Microsoft excel - data analysis
- Microsoft excel - dashboard / data visualization

## EXPLORATORY DATA ANALYSIS
### PRIMARY KPIS
* Total number of crimes recorded 
* Total number of recorded crimes and percentage of total with respect to status of case.
* Average age of victims
* Average delay report days

### sECONDARY KPIS
* Top 5 most common crimes
* Crime incident by victims gender/sex
* Crime incident by victim descent
* Crime incident by monthly trends
* Highest crime occured and percentage of the total recorded.
  
