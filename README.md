# Relationship between fish biomass and phosphorus in the Great Lakes nearshore and offshore
- Read the data from an excel file that has two sheets, "data" and "readme"
- The sheet "data" contains fish biomass information as follows:

|   |  year |  port |  depth (m) |  species |     #/ha |     g/ha |      Lat |     Long |
|---| ---   |---    | ---        |----      | ---      |---       |---       | ---       |
|0 | 1973 |  210 |   18 | 106 |  3079.45 |  9677.60 | 44.5177 | -86.2595 |
|1 | 1973 |  210 | 18 | 109 |   192.32 |  1258.37 | 44.5177 |-86.2595 |
|2 | 1973 |   210 |18 |  127 | 0.00 |  0.00 |  44.5177 | -86.2595 |

From the "readme" sheet of the excel file, we get species names and port names:
Species names:

|  | Species Code |  Species Name |
|---|---|---|
| 0 | 106 | Alewife |
|1 | 109 | Rainbow Smelt |
| 2 | 127 | Burbot |

Port names:

| |  Port No | Port Name |
|---|---|---|
| 0 |   210.0 | Frankfort, MI |
|1|    214.0 | Ludington, MI |
| 2 |   224.0 | Saugatuck, MI |
| 3 |   234.0 | Waukegan, IL |
| 4 |   240.0 | Port Washington, WI |

- We merge these three dataframes and divide the dataframe into two dataframes: nearshore and offshore
- **nearshore** has the sampling depth of less than 30m.
- **offshore** has the sampling depth of greater than or equal to 30m.
- We analyze total fish biomass by year, by different ports and species

