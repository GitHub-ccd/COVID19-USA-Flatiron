# COVID19-USA-Flatiron

COVID-19 data scraping, cleaning and analysis by dsc-03022020-Flariron cohort

## 1. Create list of state gov websites to scrape
### List of State URLS to scrape:

Base state urls, start here and dial in to find the data: https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html

- California: (entire california statistics by county) https://data.chhs.ca.gov/dataset/california-covid-19-hospital-data-and-case-statistics/resource/cd7ff27d-ac5d-419d-b850-5f6098dbfccc
- Washington: (washington stats, links to individual counties are present) https://www.doh.wa.gov/Emergencies/Coronavirus
- Colorado: (CO stats, counties are also present) https://covid19.colorado.gov/case-data
- Alabama: (includes some numbers for counties) https://alabamapublichealth.gov/infectiousdiseases/2019-coronavirus.html
- Pennsylvania: (includes counties) https://www.health.pa.gov/topics/disease/coronavirus/Pages/Cases.aspx


## 2. Create parser for each state

## 3. Build scraper and run for each state

## Ideas:
1. Include county information so we can map more specifcally

## Shape:
| ID|     State      | County  |  Lat  |  Long  | Updated  | Confirmed | Deaths | Recovered | Active |
|---|----------------|---------|-------|--------| ---------| ----------|--------|-----------|--------|
|  0| South Carolina | Horry   | 34.22 | -82.46	|2020-04-02| 6         | 0      | 0         | 0      |
