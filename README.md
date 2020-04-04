# COVID19-USA-Flatiron

COVID-19 data scraping, cleaning and analysis by dsc-03022020-Flariron cohort
## Contributing:
### Phase 1 (list of urls to scrape):
1. Fork this repository
2. Clone onto your computer
3. Pick a state that does not have a link
4. Click on this [link](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html) and find the state you chose
5. Search the state site until you find a page that lists the data per county
6. Update the site table below with the new link
7. Save and push to your github
8. Go to your github and submit a pull request

### short term objective
//TODO
able to have a bar chart race animation such as [lick](https://www.mercurynews.com/2020/04/03/watch-the-stunning-growth-of-coronavirus-cases-in-californias-hardest-hit-counties/) but for counties of each state or city


### Phase 2 (creating html parsers):
//TODO

### Phase 3 (creating scraper):
//TODO

## List of state gov websites to scrape
### List of State URLS to scrape:

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


## Parser for each states html
<code>

    use the state link to grab html:
        use html to grab info:
            result = {
                'State': html.state,
                'County': html.county,
                'Lat': find latitude using county name,
                'Long': find latitude using county name,
                'Updated': now,
                'Confirmed': html.confirmed,
                'Deaths': html.deaths,
                'Recovered': html.recovered,
                'Active': html.active,
            }
        return result
    
</code> 

## Build scraper and run for each state
<code>

    for each state:
        results = parse(state.url, state.parser)
        add results to dataset
    
    save results
    
</code>

## Additional Ideas:
1. Include county information so we can map more specifcally

## Final Data Shape:
| ID|     State      | County  |  Lat  |  Long  | Updated  | Confirmed | Deaths | Recovered | Active |
|---|----------------|---------|-------|--------| ---------| ----------|--------|-----------|--------|
|  0| South Carolina | Horry   | 34.22 | -82.46	|2020-04-02| 6         | 0      | 0         | 0      |
