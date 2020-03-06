# pythonBatchGeocoding
Python script that reads in a CSV file and geocodes a specified column into a outputted csv file.
* NB! the CSV file needs to be a semi-colon ';' delimiter seperated list.

## To install
- Please install the latest python 3 (3.8.2 was used at the time) from: https://www.python.org/downloads/ 
- install the following libraries through pip3 or whataver your preference might be:
  - pip3 install pandas (used to import and read CSV files and to create the outputted CSV file)
  - pip3 install requests
  - pip3 install click (used for the command line interface (https://click.palletsprojects.com/en/7.x/))
  
## To Run
> py pythonBatchGeocoding.py 

> Your input CSV name: (eg: data/file.csv): path/to/your/file.csv

> Name of the column for processing: (eg: Address): Address

> Your output file CSV name and directory (eg: data/outputfile.csv): path/to/save/output/file.csv

## Output 
```
             Area                               Store names                                            Address
0       Claremont                       Pick n Pay clarmont  Main Rd & Campground Rd, Claremont, Cape Town,...
1       Plumstead               Pick n Pay Family plumstead          29 Gabriel Rd, Plumstead, Cape Town, 7800
2      Kenilworth      Pick n Pay Kenilworth Clothing Store  78, 01 Doncaster Rd &, Chichester Rd, Kenilwor...
3      Kenilworth   Pick n Pay Clothing - Kenilworth Centre         Shop 78 Kenilworth Centre, Cape Town, 7745
4      Kenilworth  Pick n Pay Kenilworth Campus Convenience       101 Rosmead Ave, Kenilworth, Cape Town, 7708
5    Hanover Park            Pick n Pay Distribution Centre                          Philippi, Cape Town, 7781
6         Wynberg                        Pick n Pay Wynberg                  Main Rd, Wynberg, Cape Town, 7800
7   Ottery/Wetton                   Pick n Pay Hyper Ottery             New Ottery Rd, Ottery, Cape Town, 7800

```
```
Geocoded: Main Rd & Campground Rd, Claremont, Cape Town, 7708: OK
Geocoded: 29 Gabriel Rd, Plumstead, Cape Town, 7800: OK
Geocoded: 78, 01 Doncaster Rd &, Chichester Rd, Kenilworth, Cape Town, 7700: OK
Geocoded: Shop 78 Kenilworth Centre, Cape Town, 7745: OK
Geocoded: 101 Rosmead Ave, Kenilworth, Cape Town, 7708: OK
Geocoded: Philippi, Cape Town, 7781: OK
Geocoded: Main Rd, Wynberg, Cape Town, 7800: OK
Geocoded: New Ottery Rd, Ottery, Cape Town, 7800: OK

Finished geocoding all addresses
```

Heavy Inspiration comes from https://www.shanelynn.ie/ tutorials.
