<img src="obi_logo.png" width="275" height="100">

# Fresno Association Of Governments Area Residential Zoning Data
## Published by The Othering &amp; Belonging Institute

This data repository contains the Othering &amp; Belonging Institute's residential zoning data, originally analyzed and published in the [Single-Family Zoning in the Fresno Region Report]()  

## Citation
Nawaz, Shahan Shahid, Stephen Menendian, Samir Gambhir. 2022. *Single-Family Zoning in Fresno*. Distributed by Othering &amp; Belonging Institute. 

## About the Data
This repository includes parcel and district level shapefiles for all 15 incorporated jurisdictions, and 1 unincorporated area. Each shapefile contains a categorization of residential zoning based on the most recent publicly available zoning maps and municipal code at the time of initial analysis (Fall 2021).  

The `city_zone` field records the city's original zoning designation as found in the zoning data.  
The `zone_descp` field records the description of the `city_zone` based on the city's ordinance.  
 The `zone_cat` field records our classification of the zone into one of the following categories:  
 
 Abbreviation | Zone name | Description
------------ | ------------- | ------------- 
 SF | Single Family Residential | This includes single-family zones, low-density zones, agricultural zones (if single-family homes are permitted), and estate zones. This category usually permits detached single-family homes or two detached single-family homes on the same lot or parcel, but not duplexes. The zone is not classified as single-family residential if it only permits the following: caretaker’s residence, employee housing, or live-work units  
 MF | Multifamily Residential | Includes attached two family homes, condos, apartments, town homes, and mobile homes (parks). Additionally, if a zone’s intent allows for both single-family homes and any of the multi-family housing above, it is sorted into the multi-family category. This category does not include employee housing and student housing.  
 MIX | Mixed-use Residential | This is land designated to blend multiple uses inclusive of residential use. This includes zones that are not strictly residential but permit or conditionally permit residential uses, e.g., industrial/commercial zones where residential uses are permitted or conditionally permitted, commercial zones where residential units are allowed in commercial buildings, mixed-use zones, or office professional districts that permit single-family homes.  
 NR | Non-Residential | Land zoned for non-residential use, including commercial, industrial, public, and recreation land use  
 ND | Non-Developable | Land outside of municipal boundaries or developable land, including water, waterways, and sphere of influence land. *This category was removed from total land area for analysis.*  

The zoning categories are summarized into four larger categories which was used to create our [city zoning maps](https://belonging.berkeley.edu/fresno-region-zoning-maps), designated under the `Zoning` field: 

Zoning | Category | Include | 
------------ | ------------- | -------------
 1 | Single Family Residential | SF  
 2 | Other Residential | MF, MIX  
 0 | Non-Residential & Unknown | NR, NA  
 3 | Non-Developable | ND  

## About the Project
This residential zoning data and analysis is part of the Othering &amp; Belonging Institute's broader research on [Segregation](https://belonging.berkeley.edu/roots-structural-racism-2020), an effort to unpack the extent, dynamics, and drivers of racial segregation. 

Exclusionary, single-family zoning has long been cited as a driver for racial segregation. In order to examine the impact of single family zoning in the Fresno Area, we gathered and categorized zoning shapefiles to measure the spatial distribution and extent of restricted single family zoning, specifically as a portion of total residential land use. In [Single-Family Zoning in the Fresno Region Report](), we used this residential zoning data to analyze measures of segregation against restricted single family zoning to show the role of zoning in driving segregation. We also used this residential zoning data to assess the characteristics of communities within and outside of restricted single family zoning in the Fresno area.

## Methodology

### Data procurement: 
Zoning shapefiles for each city in the region were gathered from multiple sources, including a dataset created by [The California Governor’s Office of Planning and Research (OPR)](https://opr.ca.gov/) through grant funding provided by the U.S. Department of Defense Office of Local Defense Community Cooperation (OLDCC), and city planning/GIS or relevant departments to ensure we have the most updated shapefiles to conduct our analysis.

### Data disclaimer:
The California Governor’s Office of Planning and Research (OPR) makes no warranty, representation or guaranty as to the content, sequence, accuracy, timeliness, or completeness
of any of the data provided herein. This data has been compiled from a variety of sources, collected and maintained for different purposes, at different times. This data was compiled and
analyzed by OPR through grant funding provided by the U.S. Department of Defense Office of Local Defense Community Cooperation (OLDCC).

This information should not be used as a substitute for legal, accounting, real estate, business, tax, or other professional advice. It should not be used as a substitute for information sourced
directly from local planning authorities. The User expressly agrees that the use of the data provided herein is at the User’s sole risk.

In no event shall OPR be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the data or the use or other dealings in the data.


### Zone categorization:
We prioritized and focused on the intent and the purpose of the zone to sort the zones into one of the three categories: non-residential/unknown, single-family, and other residential. For example, a residential zone intended for both single-family and multi-family developments would be classified in the other residential category (which includes multi-family zones), even if multi-family is only conditionally permitted. This is because the zone’s intention was for both single-family and multi-family developments. 

When the intent and purpose of the zone was unclear, we classified the zone based on what is permitted in the zone. For example, consider a “general residential” zone that does not specify whether it is strictly for single-family homes in its intent. If it permits single-family homes but only conditionally permits multi-family homes, it would be classified in the single-family category. And if it permits both single-family homes and multi-family homes, it would be classified in the other residential category. Since we prioritized the zone’s stated intent and purpose in the city ordinance, we would only rely on the permitted use if the intent and purpose was unclear.

For planned development and specific plan zones where the municipal ordinance does not detail the intent and purpose enough for us to classify the entire zone or zones that are missing in the municipal ordinance, we used the standardized land use class from SCAG to categorize the parcels in these zones into one of the three categories above.

## License and Attribution
We are making this data publicly available for broad, noncommercial public use for researchers, policymakers, and the academic community. If you use this data, we request you attribute it to “The Othering &amp Belonging Institute” in your publication and use the citation provided below. If you use it in an online report, we request that you link to our our digital report, [Single-Family Zoning in the Fresno Region Report]().  

If you do use the data, we would love to hear about it! Send us an email at <belonging@berkeley.edu>

See our [LICENSE](https://github.com/OtheringBelonging/SANDAGZoning/blob/main/LICENSE) for the full terms of use for this data.

## Contact Us
If you have questions about the data or licensing conditions, please contact us at: <belonging@berkeley.edu> 
