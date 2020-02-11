# U.S. Measles Vaccination Data

This repository contains immunization rate data for schools across the U.S., as compiled by The Wall Street Journal. The dataset includes the overall and MMR-specific vaccination rates for **46,412** schools in **32** states. As used in [“What’s the Measles Vaccination Rate at Your Child’s School?“](https://www.wsj.com/graphics/school-measles-rate-map/). 

Vaccination rates are for the 2017-18 school year for Colorado, Connecticut, Minnesota, Montana, New Jersey, New York, North Dakota, Pennsylvania, South Dakota, Utah and Washington. Rates for other states are 2018-19.

It is available under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## Files

Our data is broken down into a few files:

| File  | Description |
| ------------- | ------------- |
| all-measles-rates.csv  | Data for each individual school  |
| state-overview.csv  | More generalized data by state counties or state school districts  |
| individual-states/[STATE].csv  | Same data as all-measles-rates, but seperated by state  |

## Attributes


| Attribute  | Description | Optional? |
| ------------- | ------------- | ------------- |
| index  |   |   |
| state  | School's state  |   |
| county  | School's county  | y  |
| district  | School's district  | y  |
| name  | School name  |   |
| type  | Whether a school is public, private, charter   | y  |
| enroll  | Enrollment*  | y  |
| mmr  | School's Measles, Mumps, and Rubella (MMR) vaccination rate  | y  |
| overall  | School's overall vaccination rate  | y  |
| xmed  | Percentage of students exempted from vaccination for medical reasons  | y  |
| xper  | Percentage of students exempted from vaccination for personal reasons  | y  |
| xrel  | Percentage of students exempted from vaccination for religious reasons  | y  |
| lat  | School latitude  | (only in individual state files)  |
| lng  | School longitude  | (only in individual state files)  |

_Depending on the state, enrollment is for kindergarten only or may extend to include other grades._

## Available States

We currently have data for the following **32** states.

- Arizona
- Arkansas
- California
- Colorado
- Connecticut
- Florida
- Idaho
- Illinois
- Iowa
- Maine
- Massachusetts
- Michigan
- Minnesota
- Missouri
- Montana
- New Jersey
- New York
- North Carolina
- North Dakota
- Ohio
- Oklahoma
- Oregon
- Pennsylvania
- Rhode Island
- South Dakota
- Tennessee
- Texas
- Utah
- Vermont
- Virginia
- Washington
- Wisconsin

## Sources

State education and health departments; National Center for Education Statistics; Google Maps (geocoding)

## Methodology

The vaccination data was provided by the state health departments. Addresses for about 16,000 schools in eight states were included in the original data. Locations of the remaining schools were determined by checking against the National Center for Education Statistics’ school directories or the states’ school directory using school name, city, county and/or school district. If there was no unique match, the school’s location was determined with Google Maps API using school name, state and county, city and/or school district. Duplicate locations were analyzed individually.

### Credits

This data was completed by staff of The Wall Street Journal: [Dylan Moriarty](https://twitter.com/DylanMoriarty), [Taylor Umlauf](https://twitter.com/TaylorUmlauf), & [Brianna Abbot](https://twitter.com/Brabbott42).
