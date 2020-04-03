# COVID19-USA-Flatiron

COVID-19 data scraping, cleaning and analysis by dsc-03022020-Flariron cohort

## 1. Create list of state gov websites to scrape
### List of State URLS to scrape:

Base state urls, start here and find the page that contains the data for the counties: 
https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html


| State             | Link                  |
|-------------------|-----------------------|
|Alabama | https://alabamapublichealth.gov/infectiousdiseases/2019-coronavirus.html |
|Alaska |
|Arizona|
|Arkansas|
|California| https://data.chhs.ca.gov/dataset/california-covid-19-hospital-data-and-case-statistics/resource/cd7ff27d-ac5d-419d-b850-5f6098dbfccc |
|Colorado| https://covid19.colorado.gov/case-data |
|Connecticut|
|Delaware|
|Florida|
|Georgia|
|Hawaii|
|Idaho|
|Illinois|
|Indiana|
|Iowa|
|Kansas|
|Kentucky|
|Louisiana|
|Maine|
|Maryland|
|Massachusetts|
|Michigan|
|Minnesota|
|Mississippi|
|Missouri|
|Montana|
|Nebraska|
|Nevada|
|New Hampshire|
|New Jersey|
|New Mexico|
|New York|
|North Carolina|
|North Dakota|
|Ohio|
|Oklahoma|
|Oregon|
|Pennsylvania| https://www.health.pa.gov/topics/disease/coronavirus/Pages/Cases.aspx |
|Rhode Island|
|South Carolina|
|South Dakota|
|Tennessee|
|Texas|
|Utah| https://coronavirus.utah.gov/case-counts/ |
|Vermont|
|Virginia|
|Washington| https://www.doh.wa.gov/Emergencies/Coronavirus |
|West Virginia|
|Wisconsin|
|Wyoming|


## 2. Create parser for each state

## 3. Build scraper and run for each state

## Ideas:
1. Include county information so we can map more specifcally

## Shape:
| ID|     State      | County  |  Lat  |  Long  | Updated  | Confirmed | Deaths | Recovered | Active |
|---|----------------|---------|-------|--------| ---------| ----------|--------|-----------|--------|
|  0| South Carolina | Horry   | 34.22 | -82.46	|2020-04-02| 6         | 0      | 0         | 0      |
