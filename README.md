# geomarkers  <a href='https://geomarker.io/geomarkers/'><img src='geomarker-io_hex_with_url.png' align="right" height="138.5" /></a>

### Demographic Information / Neighborhood Characteristics

The [census Block Group](https://github.com/degauss-org/census_block_group) DeGAUSS container can be used to obtain census geography identifiers in order to merge in any of the data below or other extant data indexed by census geography identifiers.

| **Geomarkers** | **Space** | **Time** | **Source** | **Software & Data Resources** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| Population, socioeconomic indicators, etc | Census tract or block | Yearly | [US Census American Community Survey (ACS)](https://www.census.gov/programs-surveys/acs/) | [hh_acs_measures](https://github.com/geomarker-io/hh_acs_measures) data resource; [harmonized_historical_census_data](https://github.com/geomarker-io/harmonized_historical_census_data) data resource; [tract_indices](https://github.com/geomarker-io/tract_indices) data resource |
| Neighborhood Deprivation Index (poverty, education, housing, and health care coverage) | Census tract or zip code | 2015, 2018 | [Material Deprivation Index](https://geomarker.io/dep_index/) | [dep index](https://github.com/geomarker-io/dep_index/tree/master/2018_dep_index#import-2018-index-directly-into-r) R code; [dep index](https://github.com/degauss-org/dep_index) DeGAUSS Container; [tract_indices](https://github.com/geomarker-io/tract_indices) data resource | 
| Child Opportunity Index (education, health & environment, social & economic neighborhood characteristics) | Census tract | 2010, 2015 | [Child Opportunity Index 2.0](https://www.diversitydatakids.org/child-opportunity-index) | [tract_indices](https://github.com/geomarker-io/tract_indices) data resource |
| Racial Index of Concentration at the Extremes (ICE) | Census tract or zip code | Yearly | [Racial ICE](https://onlinelibrary.wiley.com/doi/10.1111/ajt.16186) | [zctaDB](https://geomarker.io/zctaDB/) R package; [tract_indices](https://github.com/geomarker-io/tract_indices) data resource | 
| Relative crime risk by crime subtype | Census block group | Average (2010 - 2017) | [AGS Crime Risk](https://appliedgeographic.com/crimerisk/) | *proprietary product for purchase from AGS.*|
| Fraction of food retailers that are "healthy" | Census tract | 2011 | [Modified Retail Food Environment Index (mRFEI)](https://www.cdc.gov/obesity/downloads/census-tract-level-state-maps-mrfei_TAG508.pdf) | [tract_indices](https://github.com/geomarker-io/tract_indices) data resource | 
| Social Vulnerability Index | County / Census tract | 2000, 2010, 2014, 2016, 2018 | [Agency for Toxic Substances and Disease Registry (ATSDR)](https://www.atsdr.cdc.gov/placeandhealth/svi/index.html) |[tract_indices](https://github.com/geomarker-io/tract_indices) data resource|
| Community Resilience Estimates | County / Census tract | Current | [US Census](https://www.census.gov/data/experimental-data-products/community-resilience-estimates.html) |[tract_indices](https://github.com/geomarker-io/tract_indices) data resource| 
| Social Deprivation Index (Area level deprivation based on ACS data) | County, census tract, ZCTA and PCSA | 2015 | [Robert Graham Center](https://www.graham-center.org/rgc/maps-data-tools/sdi/social-deprivation-index.html) |[tract_indices](https://github.com/geomarker-io/tract_indices) data resource|

### Air Pollution

| **Geomarkers** | **Space** | **Time** | **Source** | **Software & Data Resources** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| PM2.5 | 0.74 sq km h3 hexagonal grid | daily (2000 - 2020) | [Brokamp exposure model](https://github.com/geomarker-io/st_pm_hex) | [addPmData](https://geomarker.io/addPmData/) R package; [pm](https://github.com/degauss-org/pm) DeGAUSS container | 
| PM2.5, NO2, O3 | 1 sq km grid | daily (2000 - 2016) | Schwartz exposure model | [schwartz](https://degauss.org/degauss_schwartz_guide/) DeGAUSS container | 
| air toxics cancer risk, respiratory hazard index, diesel PM, PM2.5, ozone, traffic proximity and volume, lead paint indicator, proximity to RPM sites, proximity to hazardous waste facilities, proximity to NPL sites, wastewater discharge indicator | Census block groups | Annual (2015 - 2020) | [EPA EJ Screen](https://www.epa.gov/ejscreen/overview-environmental-indicators-ejscreen) | [zctaDB](https://geomarker.io/zctaDB/) R package | 
| Location and amount of emissions | Exact location |	Yearly (2008, 2011, 2014, 2017) | [National Emissions Inventory (NEI)](https://www.epa.gov/air-emissions-inventories/national-emissions-inventory-nei) | | 
| PM2.5, PM10, O3, CO, SO2, NO2 | Census block group (Contiguous US) | Annual (1999 - 2015) | [CACES LUR](https://www.caces.us/data) | |
| PM2.5, SO4, NO3, NH4, OM, BC, DUST, SS | 0.01° × 0.01° (North America) | Annual (2000 - 2018) | [ACAG MAPLE](http://fizz.phys.dal.ca/~atmos/martin/?page_id=140) | |
| PM2.5, GBD-MAPS, NO2, Inverse Visibility, OM/OC, Surface Area, NOy Deposition, Dry Deposition, AMF Code | 0.01° × 0.01° (North America) | Annual / Monthly | [ACAG Washington University in St. Louis](https://sites.wustl.edu/acag/datasets/)
| PM2.5, NO2 | Tract Centers (Contiguous US) | Monthly (1999 – 2008) | Beckerman | |

### Environmental Exposures

| **Geomarkers** | **Space** | **Time** | **Source** | **Software & Data Resources** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| Air temperature, planetary boundary height, relative humidity, precipitation, wind |	North America (0.3°×0.3°) |	8-times a day (2001 – current); daily means (1979 – current) |	[North American Regional Reanalysis (NARR)](https://www.ncdc.noaa.gov/data-access/model-data/model-datasets/north-american-regional-reanalysis-narr) | [addNarrData](https://geomarker.io/addNarrData/) R package;  [narr](https://degauss.org/narr/) DeGAUSS container |
| Greenspace as Enhanced Vegetation Index (EVI) | 250 × 250 m grid (contiguous US) | June 10 and June 25, 2018 composite | [Moderate Resolution Imaging Spectroradiometer (MODIS)](https://search.earthdata.nasa.gov/search) | [greenspace](https://degauss.org/greenspace/) DeGAUSS container |
| Land cover classifications (21 classes) |	30 x 30 m grid |	Annual (2001, 2006, 2011, 2016) |	[National Land Cover Database (NLCD)](https://www.mrlc.gov/) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Fractional imperviousness	| 30 x 30 m grid |	Annual (2001, 2006, 2011, 2016) |	[NLCD Imperviousness](https://www.mrlc.gov/data/nlcd-2016-percent-developed-imperviousness-conus) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Roadway type, development intensity |	30 x 30 m grid |	Annual (2001, 2006, 2011, 2016) |	[NLCD Imperviousness Classification](https://www.mrlc.gov/data/nlcd-2016-developed-imperviousness-descriptor-conus) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Vegetation Type |	30 x 30 m grid | Annual (2011, 2016) |	[NLCD Tree Canopy](https://www.mrlc.gov/data/nlcd-2016-usfs-tree-canopy-cover-conus) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Greenspace as fraction of land classified as green | 30 x 30 m grid	| Annual (2001, 2006, 2011, 2016)	| [NLCD Greenness](https://www.mrlc.gov/data/nlcd-land-cover-conus-all-years) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Highway traffic intensity	| Exact location (nationwide) |	Yearly |	[US Department of Transportation (DOT)](https://www.transportation.gov/) | [addAadtData](https://geomarker.io/addAadtData/) R package; [aadt](https://degauss.org/aadt/) DeGAUSS container | 
| Noise level |	270 m sq grids (nationwide) |	2015 |	[National Park Service Geospatial Sound Modeling (GSM)](https://www.nps.gov/subjects/sound/soundmap.htm) | |

### Greater Cincinnati Area Only

| **Geomarkers** | **Space** | **Time** | **Source** | **Software & Data Resources** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| Parcel classification and characteristics |	Exact location (Greater Cincinnati Area) | Current | [Cincinnati Area Geographic Information Systems (CAGIS)](http://cagis.org/Opendata/?) |  |
| Home images, value, age, other physical characteristics, owner name | Exact |	Exact	Inspection dates |	[Hamilton County Auditor](https://wedge.hcauditor.org/)	| [hamilton](https://github.com/geomarker-io/hamilton) R package for parcel-based geocoding |	
| Traffic Related Air Pollution	| Exact location (seven county area served by CCHMC) |	Monthly (2001 – current) |	[Air pollution exposure model](https://doi.org/10.1289/ehp.9480) |	[ecat](https://geomarker.io/ecat/) R package |
| PM2.5 components: Al, Cu, Fe, K, Mn, Pb, S, Si, V, Zn | Exact location |	Average daily exposure (2002-2006) |	[Air pollution exposure model](http://dx.doi.org/10.1016/j.atmosenv.2016.11.066) |   |
| Lead Air Pollution |	Exact location (seven county area served by CCHMC) |	Monthly (2001 – current) |	[Air pollution exposure model](http://dx.doi.org/10.1016/j.atmosenv.2016.11.066) |	[airPb](https://geomarker.io/airPb) R package	|
| Estimated travel time by car |	Census tract and traffic analysis area |	Hourly (2016-2017) |	[Uber Move](https://movement.uber.com/explore/cincinnati/travel-times/query?si=156&ti=&ag=censustracts&dt[tpb]=ALL_DAY&dt[wd;]=1,2,3,4,5,6,7&dt[dr][sd]=2019-12-01&dt[dr][ed]=2019-12-31&cd=&sa;=&sdn=&lang=en-US	)	| |
| Combined Sewer Overflow events |	Exact location |	Daily (2012 - 2016) |	Metropolitan Sewer District (MSD) | |
| Areas without access to medication-assisted treatment and/or behavioral therapy for opioid addiction |	Exact location (seven county area served by CCHMC) |	2019 |	MAT Desert | [MAT Desert shapfiles](https://zenodo.org/record/4011051) |			
| Crime |	Exact location (Ohio) |	Annual (2013 - 2018)|	[Ohio Incident Based Reporting System](https://www.ocjs.ohio.gov/crime_stats_reports.stm#gsc.tab=0) | |
