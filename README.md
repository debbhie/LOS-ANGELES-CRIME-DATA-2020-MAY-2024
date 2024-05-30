# LOS-ANGELES-CRIME-DATA-2020-MAY-2024

## TABLE OF CONTENT
- [LOS ANGELES CRIME DATA 2020 - MAY 2024 OVERVIEW](los-angeles-crime-data-2020-may-2024)
- [DATA SOURCE](data-source)
- [LANDING PAGE](landing-page)
- [TOOLS](tools)
- [EXPLORATORY DATA ANALYSIS](exploratory-data-analysis)
- [DATA CLEANING](data-cleaning)
- [DATA PROCESSING](data-processing)
- [DATA ANALYSIS](data-analysis)
- [DATA VISUALIZATION](data-visualization)
- [INSIGHTS](insights)
- [RECOMMENDATIONS](recommendations)


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

### SECONDARY KPIS
* Top 5 most common crimes
* Crime incident by victims gender/sex
* Crime incident by victim descent
* Crime incident by monthly trends
* Highest crime occured and percentage of the total recorded.
* Crime incident by victims age range
* Top 10 crime premises description
* Crime incident occured by area name

## DATA CLEANING
These processes were carried out using power query
* No duplicates were found in the dataset
* The null values were replaced with "no record" because there are no constant values and the informations missing were very important to ensure accurate analysis.

## DATA PROCESSING
* Months of the year were extracted from the date columns.
* Report delay days column was created by using function (days) on excel to extract number of days it took for the crime to be reported.

## DATA ANALYSIS
 
### PRIMARY KPIS
* Total number of recorded crimes between 2020 to may 2024 is 944,235.

* Percentage of total crimes recorded with respect to status of case:
   * Adult Arrest: 82,182 (9%)
   * Adult other: 102,928 (11%)
   * Investigation continues: 754,264 (80%)
   * Juvenile arrest: 3,102
   * Juvenile other; 1,754
   * Unkonwn: 5

* Average age of victims: 56years old.

* Average report delay days: 692days

### SECONDARY KPIS
* Top 5 common crimes
 * Vehicle-stolen: 102,203
 * Battery-simple assault: 74,500
 * Burglary from vehicle: 58,300
 * Theft of Identity: 58,200
 * Burglary: 57,200

* Crime incident by victims gender/sex
   * Male: 385,800
   * Female: 344,400
   * Unknown: 87,700
   * No record: 126,600

* Crime incident by victims age range
   * -4-5years: 242,200
   * 26-35years: 198,100
   * 36-45years: 146,300
   * 16-25years: 116,200
   * 46-55years: 105,300
   * 56-65years: 73,100
   * 66-75years: 33,800
   * 6-15years: 105,300
   * 76-85years: 11,100
   * 86-95years: 2,500
   * 96-105years: 600
   * 116-125years: 0

* Crime incident by victims descent
   * Hispanic/latino/mexican (H): 286,400
   * White (W): 190,500
   * Black (B): 131,700
   * No record: 126,600
   * Unknown (X): 96,200
   * Others: 74,400
   * Other Asian (A): 20,600
   * kOREAN (K): 5,200
   * Filipino (F): 4,100
   * Chinese (C): 3,800
   * Japanese (J): 1,300
   * Vietnamese (V): 1,000
   * American indian/Alaskan native (I): 900
   * Asian indian (Z): 500
   * Pacific Islander (P): 300
   * Hawaiian (u): 200
   * Cambodian (D): 100
   * Guamanian (G): 100
   * Laotian (L): 100
   * Samoan (S): 100
   * Uknown: 0

  * Crime incident by monthly trends
    * Lowest crime month: february 2021 with the total recorded crimes of 15,427
    * Highest crime month: may 2022 with the total recorded crimes of 20,450

  * Highest crime type:
     vehicle-stolen with the total of 102,203

* Top 10 crime premises
   * Street: 240,300
   * Single family dwelling: 158,900
   * Multi unit dwelling: 114,800
   * Parking lots: 65,200
   * Other business: 45,000
   * Side walks: 39,900
   * Vehicle/passenger/truck: 27,500
   * Garage/Carpots: 18,100
   * Driveway: 15,000
   * Department store: 12,600

* Crime incident by Area name:
   * Central: 63,700
   * 77th street: 59,200
   * Pacific: 55,000
   * Southwest: 53,500
   * Hollywood: 49,500
   * North Hollywood: 47,900

### OVERVIEW OF CRIME DATA BY YEAR AND GENDER/SEX
|Crime Recorded| Gender/Sex| 2020| 2021| 2022| 2023| 2024|
|--------------|-----------|-----|------|------|------|-----|
|Total Recorded Crimes| female| 72,645| 77,002| 89,500| 82,683| 22,317|
|                     | male| 84,942| 88,073| 95,654| 91,495|25,605|


| Crime Recorded | Gender/Sex | 2020| 2021| 2022| 2023| 2024|
|----------------|------------|-----|-----|-----|-----|-----|
|case status|
| Investigation Continues| female| 49,615| 54,227| 67,054| 62,878| 19,165|
|Investigation Continues| male| 65,538| 69,460| 77,206| 74,156| 22,395|
|Adult Arrest| female| 8,724| 8,523| 8,122| 7,057| 1,271|
| Adult Arrest| male| 8,522| 8,151| 8,226| 7,605| 1,666|
| Adult Other| female| 13,845| 13,812| 13,879| 12,247| 1,781|
| Adult other| male| 10,431| 10,035| 9,691| 9,151| 1,366|


| Crime level| Crime Month| total crime|Gender/sex| Year|
|------------|-------------|-----------|----------|-----|
| Highest| february| 6,675| female| 2020|
| lowest| April| 5,554| female| 2020|
| highest| january| 8,020| male| 2020|
| lowest| April and september|6,581|  male| 2020|
| highest| october| 7,173|female| 2021|
| lowest| february| 6,751| female| 2021|
| highest| july| 8,047| male| 2021|
| lowest| february| 6,434| male| 2021|
| highest| october|7,860|female| 2022|
| lowest| february| 6,751| female| 2022|
| highest| june| 8,304| male| 2022|
| lowest| november| 7,468| male| 2022|
| highest| january| 7,530| female| 2023|
| lowest| november| 6,384| female| 2023|
| highest| july| 8,014| male| 2023|
| lowest| november| 7,344| male| 2023|
| highest|january| 6,047| female| 2024|
| lowest| may| 1,121| female| 2024|
| highest| january| 7,301| male| 2024|
| lowest| may| 1,371| male| 2024|

## DATA VISUALIZATION


## INSIGHTS
* CRIME TRENDS:
  * There is a high volume of vehicle-related crimes, particularly vehicle theft.
  * Crime tends to peak in the summer months and around holiday seasons.

* VICTIMS DEMOGRAPHICS:
   * A significant number of crimes involve younger adults aged 26-35.
   * Hispanic/latino/mexican victims constitute the largesr ethnic group among recorded crimes.

* CASE STATUS:
   * The vast majority of the cases remain under investigation, indicating potential bottle necks or resource constraints within investigative processes.

* REPORT DELAYS: The average delay in reporting crimes is alarming high, with significant delays in some cases exceeding a year.

* GENDER DISPARITIES:
   * There are noticeable differences in crime typrs and frequencies between male and female victims. For example, intimate partner assault is significantly high in female while assault with deadly weapon is high in male.


## RECOMMENDATIONS
* ENHANCE DATA COLLECTION AND CATEGORIZATION:
  * Improve the accuracy and completness of data recording, especially for victims demographics and case statuses.
  * Implement standardized data entry protocols across all precinctd to ensure consistency.
 
* REDUCE REPORTING DAYS:
  * Develop and promote public awareness campaigns to encourage timely reporting of crimes.
  * Implement streamlined reporting systems, including online and mobile platforms, to make it easier for victims to report incidents.

* TARGETED CRIME PREVENTION STRATEGIES:
  * Focus on high incident crimes such as vehicle theft and battery-simple assault with targeted prevention and intervention programs.
  * Increase police presence and surviellance in high crime areas like central, 77th street and pacific to deter criminal activities.

* SUPPORT FOR VULNERABLE DEMOGRAPHICS:
  * Provide additional resources and support service for demographics with high crime victimization rate such as hispanic/latino/mexican descent communities and younger victims'.
  * Develop specialized programs for crime prevention and victims support tailored to the needs of these communities.

 * IMPROVE PREMISES SECURITY:
     * Work with local businesses and residential areas to enhance security measures in top crime premises like street, single-family and multi-unit dwellings.
     * Promote community-based initiatives such as neighborhood watch programs to increase vigilance and reporting.
  
  * MONTHLY CRIME PATTERN ANALYSIS:
     * Conduct monthly analysis of crime trends to identify and respond to emerging patterns promptly.
     * Allocate resources dynamically based on monthly crime fluctuations to address peak crime periods effectively.

  * ENHANCE INVESTIGATION AND CASE RESOLUTION:
     * Allocate more resources to expedite ongoing investigations, aiming to reduce the backlogs of unresolved cases.
     * Implement training programs for law enforcement officers to improve investigation techniques and case management.
    





