# geomarkers

### Demographic Information / Neighborhood Characteristics

| **Geomarkers** | **Space** | **Time** | **Source** | **Available DeGAUSS Products** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| Population, socioeconomic indicators, etc | Census tract or block | Yearly | [US Census American Community Survey (ACS)](https://www.census.gov/programs-surveys/acs/) | |
| Neighborhood deprivation index (poverty, education, housing, and health care coverage) | Census tract or zip code | 2015, 2018 | [Neighborhood Deprivation Index](https://geomarker.io/dep_index/) | coming soon | 
| Child Opportunity Index (education, health & environment, social & economic neighborhood characteristics) | Census tract | 2010, 2015 | [Child Opportunity Index 2.0](https://www.diversitydatakids.org/child-opportunity-index) | |
| Racial Index of Concentration at the Extremes (ICE) | Census tract or zip code | Yearly | [Racial ICE](https://onlinelibrary.wiley.com/doi/10.1111/ajt.16186) | [zctaDB](https://geomarker.io/zctaDB/) R package | 
| Relative crime risk by crime subtype | Census block group | Average (2010 - 2017) | [AGS Crime Risk](https://appliedgeographic.com/crimerisk/) | |
| Location and type of gun violence incident | Exact | Annual (2014 - current) | [Gun Violence Archive (GVA)](https://www.gunviolencearchive.org/) | |
| Fraction of food retailers that are "healthy" | Census tract | 2011 | [Modified Retail Food Environment Index (mRFEI)](https://www.cdc.gov/obesity/downloads/census-tract-level-state-maps-mrfei_TAG508.pdf) | | 
| Food access indicators, SNAP benefits, demographics | Census tract | 2015 | [USDA Food Access Research Atlas](https://www.ers.usda.gov/data-products/food-access-research-atlas/) | |
| Medically Underserved Areas | County / Census tract | Current | [Health Resources and Services Administration (HRSA)](https://data.hrsa.gov/data/download) | [MUA App](https://erikarasnick.shinyapps.io/mua_app/) | 
| Location and financial operations of non-profit organizations | Exact | Annual (1989 - 2013) | [National Center for Charitable Statistics (NCCS)](https://nccs-data.urban.org/index.php#page-top) | |

### Air Pollution

| **Geomarkers** | **Space** | **Time** | **Source** | **Available DeGAUSS Products** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| PM2.5 | 0.74 sq km h3 hexagonal grid | daily (2000 - 2020) | coming soon | coming soon | 
| air toxics cancer risk, respiratory hazard index, diesel PM, PM2.5, ozone, traffic proximity and volume, lead paint indicator, proximity to RPM sites, proximity to hazardous waste facilities, proximity to NPL sites, wastewater discharge indicator | Census block groups | Annual (2015 - 2020) | [EPA EJ Screen](https://www.epa.gov/ejscreen/overview-environmental-indicators-ejscreen) | [zctaDB](https://geomarker.io/zctaDB/) R package | 
| Fixed site monitoring of ambient pollutant levels, air quality alerts |	Interpreted from over 2500 stations (nationwide) | Daily | [EPA Air Quality System (AQS)](https://aqs.epa.gov/aqsweb/airdata/download_files.html) | |
| Location and amount of emissions | Exact location |	Yearly (2008, 2011, 2014, 2017) | [National Emissions Inventory (NEI)](https://www.epa.gov/air-emissions-inventories/national-emissions-inventory-nei) | | 
| PM2.5, PM10, O3, CO, SO2, NO2 | Census block group (Contiguous US) | Annual (1999 - 2015) | [CACES LUR](https://www.caces.us/data) | |
| PM2.5, SO4, NO3, NH4, OM, BC, DUST, SS | 0.01° × 0.01° (North America) | Annual (2000 - 2018) | [ACAG MAPLE](http://fizz.phys.dal.ca/~atmos/martin/?page_id=140) | |
| PM2.5, NO2 | Tract Centers (Contiguous US) | Monthly (1999 – 2008) | Beckerman | |

### Environmental Exposures

| **Geomarkers** | **Space** | **Time** | **Source** | **Available DeGAUSS Products** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| Air temperature, planetary boundary height, relative humidity, precipitation, wind |	North America (0.3°×0.3°) |	8-times a day (2001 – current); daily means (1979 – current) |	[North American Regional Reanalysis (NARR)](https://www.ncdc.noaa.gov/data-access/model-data/model-datasets/north-american-regional-reanalysis-narr) | [addNarrData](https://geomarker.io/addNarrData/) R package;  [narr](https://degauss.org/narr/) DeGAUSS container |
| Temperature, relative humidity, precipitation, wind speed and direction	| Interpreted from > 5000 stations (nationwide) |	[Daily	Global Historical Climatology Network (GHCN)](https://www.ncdc.noaa.gov/data-access/land-based-station-data/land-based-datasets/global-historical-climatology-network-ghcn) | |
| Greenspace, aerosol optical thickness, surface reflectance | 1 km square grids (nationwide)	| Daily (2000 – current) | [Moderate Resolution Imaging Spectroradiometer (MODIS)](https://search.earthdata.nasa.gov/search) | |
| Greenspace as Enhanced Vegetation Index (EVI) | 250 × 250 m grid (contiguous US) | June 10 and June 25, 2018 composite | [Moderate Resolution Imaging Spectroradiometer (MODIS)](https://search.earthdata.nasa.gov/search) | [greenspace](https://degauss.org/greenspace/) DeGAUSS container |
| Land cover classifications (21 classes) |	30 x 30 m grid |	Annual (2001, 2006, 2011, 2016) |	[National Land Cover Database (NLCD)](https://www.mrlc.gov/) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Fractional imperviousness	| 30 x 30 m grid |	Annual (2001, 2006, 2011, 2016) |	[NLCD Imperviousness](https://www.mrlc.gov/data/nlcd-2016-percent-developed-imperviousness-conus) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Roadway type, development intensity |	30 x 30 m grid |	Annual (2001, 2006, 2011, 2016) |	[NLCD Imperviousness Classification](https://www.mrlc.gov/data/nlcd-2016-developed-imperviousness-descriptor-conus) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Vegetation Type |	30 x 30 m grid | Annual (2011, 2016) |	[NLCD Tree Canopy](https://www.mrlc.gov/data/nlcd-2016-usfs-tree-canopy-cover-conus) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Greenspace as fraction of land classified as green | 30 x 30 m grid	| Annual (2001, 2006, 2011, 2016)	| [NLCD Greenness](https://www.mrlc.gov/data/nlcd-land-cover-conus-all-years) | [addNlcdData](https://geomarker.io/addNlcdData/) R package;  [nlcd](https://degauss.org/nlcd/) DeGAUSS container |
| Location efficiency, characteristics of the built environment |	Census tract | 2010 |	[Smart Location Database (SLD)](https://www.epa.gov/smartgrowth/smart-location-mapping) | |
| Highway traffic intensity	| Exact location (nationwide) |	Yearly |	US Department of Transportation (DOT) | | 
| Quantity of types of animals, products, crops |	Zip Code | 1997, 2002, 2007, 2008, 2011 - 2016 | [USDA National Agricultural Statistics Service (NASS)](https://www.nass.usda.gov/) | |
| Highway traffic intensity	| Exact location (nationwide) |	Yearly |	[US Department of Transportation (DOT)](https://www.transportation.gov/) | | 
| Noise level |	270 m sq grids (nationwide) |	2015 |	[National Park Service Geospatial Sound Modeling (GSM)](https://www.nps.gov/subjects/sound/soundmap.htm) | |



### Greater Cincinnati Area Only

| **Geomarkers** | **Space** | **Time** | **Source** | **Available DeGAUSS Products** |
| --------------------- | ---------------------------- | --------- | --------- | --------- |
| Crime density, combined sewer overflow sites, housing infractions, urban tree cover, etc |	Exact location (Greater Cincinnati Area) | Current | [Cincinnati Area Geographic Information Systems (CAGIS)](http://cagis.org/Opendata/?) | [hamilton](https://github.com/geomarker-io/hamilton) R package for parcel-based geocoding |
|Estimated travel time by car |	Census tract and traffic analysis area |	Hourly (2016-2017) |	[Uber Move](https://movement.uber.com/explore/cincinnati/travel-times/query?si=156&ti=&ag=censustracts&dt[tpb]=ALL_DAY&dt[wd;]=1,2,3,4,5,6,7&dt[dr][sd]=2019-12-01&dt[dr][ed]=2019-12-31&cd=&sa;=&sdn=&lang=en-US	)	| |
| Combined Sewer Overflow events |	Exact location |	Daily (2012 - 2016) |	Metropolitan Sewer District (MSD) | |
| Home images, value, age, other physical characteristics, owner name |	Exact	Inspection dates |	Hamilton County Auditor	| |	
| Land cover in 6 categories: impervious, tree canopy, agriculture, bare soil, grass/meadow, water |	1 x 1 m (Cincinnati and Northern Kentucky) |	2010 |	Urban Tree Canopy (UTC) Assessments | |		
| Satellite measured near-infrared and visible radiation |	30 x 30 m (seven county region) |	2000 & 2010	Normalized Differential Vegetation (NDVI) cover	| |		
| Vacant properties, managed and vouchered properties, management companies |	Exact location (Greater Cincinnati Area) |	Current	 | Cincinnati Metro Housing Authority (CMHA) |  |
| PM2.5 components: Al, Cu, Fe, K, Mn, Pb, S, Si, V, Zn | Exact location |	Average daily exposure (2002-2006) |	[Air pollution exposure model](http://dx.doi.org/10.1016/j.atmosenv.2016.11.066) |   |
| PM2.5 |	Exact location (seven county area served by CCHMC) |	Daily (2000 – 2015)	 | [Air pollution exposure model](https://doi.org/10.1021/acs.est.7b05381) |	[aiR](https://geomarker.io/aiR/) package |
| Traffic Related Air Pollution	| Exact location (seven county area served by CCHMC) |	Monthly (2001 – current) |	[Air pollution exposure model](https://doi.org/10.1289/ehp.9480) |	[ecat](https://geomarker.io/ecat/) package |
| Lead Air Pollution |	Exact location (seven county area served by CCHMC) |	Monthly (2001 – current) |	[Air pollution exposure model](http://dx.doi.org/10.1016/j.atmosenv.2016.11.066) |	[airPb](https://geomarker.io/airPb) package	|
| Areas without access to medication-assisted treatment and/or behavioral therapy for opioid addiction |	Exact location (seven county area served by CCHMC) |	2019 |	MAT Desert |  |			
| Crime |	Exact location (Ohio) |	Annual (2013 - 2018)|	[Ohio Incident Based Reporting System](https://www.ocjs.ohio.gov/crime_stats_reports.stm#gsc.tab=0) | |
