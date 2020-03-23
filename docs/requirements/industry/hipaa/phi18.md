# PHI data type requirements

## Names

Person names are supported by Presidio with the standard recognizer.

## Geographical location

The official description of protected location information is:

> All geographical subdivisions smaller than a State, including street address, city, county, precinct, zip code, and their
> equivalent geocodes, except for the initial three digits of a zip code, if according to the current publicly available data
> from the Bureau of the Census: (1) The geographic unit formed by combining all zip codes with the same three initial digits
> contains more than 20,000 people; and (2) The initial three digits of a zip code for all such geographic units containing
> 20,000 or fewer people is changed to 000.

The general case includes:

- Street addresses in US style, such as `<number> <street name> [<town>] [<zip code>] [<state>]`
- US city names
- US county names
- US precinct names
- Bare zip codes
- Location codes in any of these formats:
  - Geolocation (longtitude/latitude) in ISO-6709 ([official](https://www.iso.org/standard/39242.html),
  [Wikipedia](https://en.wikipedia.org/wiki/ISO_6709)) formats
  - [Geohash](https://en.wikipedia.org/wiki/Geohash)
  - [Open Location Codes](https://en.wikipedia.org/wiki/Open_Location_Code)
  - [What3words codes](https://what3words.com/)
  - [Mapcodes](https://www.mapcode.com/)

## TBD

Dates directly related to an individual (see [Identifiers list](#identifiers-list) for details)
Phone numbers
Fax numbers
E-mail addresses
Social Security numbers
Medical record numbers
Health plan beneficiary numbers
Account numbers
Certificate/license numbers
Vehicle identifiers and serial numbers, including license plate numbers
Device identifiers and serial numbers
URLs
IP address numbers
Biometric identifiers, including finger and voice prints
Full face photographic images and any comparable images
Any other unique identifying number, characteristic, or code
