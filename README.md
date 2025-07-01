# Dataset for the Geospatial Data Carpentry for Urbanism

## Table of Contents

- [1. GENERAL INFORMATION](#1-general-information)
    - [1.1 Title of Dataset](#11-title-of-dataset)
    - [1.2 Dataset description](#12-dataset-description)
    - [1.3 Authors Information](#13-authors-information)
    - [1.4 Dates of data collection](#14-dates-of-data-collection)
    - [1.5 Geographic location of data collection](#15-geographic-location-of-data-collection)
    - [1.6 Keywords](#16-keywords)
    - [1.7 Language](#17-language)
    - [1.8 Information about funding sources that supported the collection of the data](#18-information-about-funding-sources-that-supported-the-collection-of-the-data)
- [2. METHODOLOGICAL INFORMATION](#2-methodological-information)
    - [2.1 Research questions, methods and envisioned uses](#21-research-questions-methods-and-envisioned-uses)
    - [2.2 Methods for processing the data](#22-methods-for-processing-the-data)
    - [2.3 Instrument- or software-specific information](#23-instrument--or-software-specific-information)
- [3. FILE OVERVIEW](#3-file-overview)
    - [3.1 File List](#31-file-list)
    - [3.2 File formats and naming conventions](#32-file-formats-and-naming-conventions)
- [4. DATA-SPECIFIC INFORMATION](#4-data-specific-information)
    - [4.1 Tabular data](#41-tabular-data)
    - [4.2 Vector data](#42-vector-data)
    - [4.3 Raster data](#43-raster-data)
- [5. SHARING/ACCESS INFORMATION](#5-sharingaccess-information)
    - [5.1 Licenses/restrictions placed on the data](#51-licensesrestrictions-placed-on-the-data)
    - [5.2 Links to other resources](#52-links-to-other-resources)
    - [5.3 Recommended citation for this dataset](#53-recommended-citation-for-this-dataset)


# 1. GENERAL INFORMATION

## 1.1 Title of Dataset
Geospatial Data Carpentry for Urbanism Workshop Data

## 1.2 Dataset description

This dataset contains geospatial data required to render the Geospatial Data Carpentry for Urbanism developed by the Rbanism team at TU Delft.

The workshop material can be accessed [here](https://carpentries-incubator.github.io/r-geospatial-urban/).

## 1.3 Authors Information
The carpentry was developed by:

- [Claudiu Forgaci](https://github.com/cforgaci)
- [Clémentine Cottineau](https://github.com/ClementineCttn)
- [Aleksandra Wilczynska](https://github.com/alwil)
- [Ana Petrovic](https://github.com/ana-5r)
- [Daniele Cannatella](https://github.com/dcannatella)
- [Ignacio Urria Yáñez](https://github.com/iurriayanez)
- [Javier San Millán Tejedor](https://github.com/javisanmillan)
- [Jerome Francisco Conceicao](https://github.com/fcjerome)
- [Kyri Janssen](https://github.com/KyriJanssen)
- [Manuel Garcia](https://github.com/manuGil)
- [Selin Kubilay](https://github.com/Selkubi)

## 1.4 Dates of data collection
January 2024

## 1.5 Geographic location of data collection
Delft, The Netherlands

## 1.6 Keywords
Geospatial, R, Urbanism, Data Carpentry, Open Data, Open Science

## 1.7 Language
English

## 1.8 Information about funding sources that supported the collection of the data
The activities of the Rbanism community, including the preparation of this
dataset, were supported by the the Netherlands eScience Center, the
Mainstreaming Open Science Fund of the Open Science Community Delft, and the
Department of Urbanism at TU Delft.

# 2. METHODOLOGICAL INFORMATION
## 2.1 Research questions, methods and envisioned uses
The dataset is designed to support the Geospatial Data Carpentry for Urbanism,
which aims to teach participants how to work with geospatial data in R,
specifically in the context of urban studies.

The dataset is structured to facilitate hands-on learning and practical
applications of geospatial analysis techniques.

## 2.2 Methods for processing the data
- Raster data was processed using the `terra` package in R.
- Vector data was processed using the `sf` package in R.
- Data was cleaned and transformed using the `dplyr` and `tidyr` packages
- Data visualization was performed using the `ggplot2` package.

## 2.3 Instrument- or software-specific information
- The workshop uses R as the primary programming language for data analysis and visualization.
- The dataset is compatible with R version 4.4.0 and above.
- The following R packages and libraries are required for the carpentry:
  - GDAL, GEOS, and PROJ.4
  - `tidyverse` v.2.0 for data manipulation and visualisation 
  - `terra` v.1.7 for handling spatial raster data
  - `sf` v.1.0 for handling spatial vector data
  - `leaflet` for interactive maps
  - `osmdata` for accessing OpenStreetMap data

# 3. FILE OVERVIEW
Are there multiple versions of the dataset? No

## 3.1 File List

### 3.1.1 Tabular data
- "gapminder-data.csv": Tabular dataset containing country-level statistics on life expectancy, population, and GDP per capita over time.

### 3.1.2 Vector data 
- "delft-boundary.shp": A shapefile with a polygon representing the boundary of the city of Delft, The Netherlands.
- "delft-leisure.shp": A shapefile with points representing leisure facilities in Delft.
- "delft-streets.shp": A shapefile with lines representing the street network in Delft.
- "nl-gemeenten.shp": A shapefile with multipolygons representing contiguous boundaries of the municipalities in the Netherlands.
- "nl-boundary.shp": A shapefile with a multipolygon representing the boundary of the Netherlands.
- "bounding-box-brielle.shp": A shapefile with a polygon representing the bounding box of the Brielle area in the Netherlands.
- "data-brielle.shp": A shapefile with polygons representing buildings in the Brielle area.

> **Note:** All shapefiles are accompanied by their standard complementary files (e.g., `.shx`, `.dbf`, `.prj`). For simplicity, only the main `.shp` file are listed here, but all associated files are included in the dataset package.


### 3.1.3 Raster data
- "tud-dsm-5m.tif": A raster dataset representing a digital surface model (DSM) of the TU Delft campus at a 5-meter resolution.
- "tud-dtm-5m.tif": A raster dataset representing a digital terrain model (DTM) of the TU Delft campus at a 5-meter resolution.
- "tud-dsm-5m-hill.tif": A hillshade raster dataset derived from the digital surface model (DSM) of the TU Delft campus.
- "tud-dtm-5m-hill.tif": A hillshade raster dataset derived from the digital terrain model (DTM) of the TU Delft campus.
- "tud-dtm-5m-hill-WGS84.tif": A hillshade raster dataset derived from the digital terrain model (DTM) of the TU Delft campus, projected in WGS 84 coordinate system.
- "tudlib-rgb.tif": A raster dataset representing the RGB (Red, Green, Blue) color composite of the TU Delft library area.


## 3.2 File formats and naming conventions
### 3.2.1 File formats
- shp - Shapefile format for vector data
- csv - Comma-separated values format for tabular data
- tif - Tagged Image File Format for raster data
- cpg - Character encoding file for shapefiles
- dbf - Database file for shapefiles
- prj - Projection file for shapefiles
- shx - Shape index file for shapefiles
- qmd - Quarto markdown file 

### 3.2.2 Naming conventions
- files named lower case, spaces replaced with dashes (dash-case)

# 4. DATA-SPECIFIC INFORMATION

- Missing data code: NA
- Not Applicable: N/A

## 4.1 Tabular data

### 4.1.1 gapminder-data.csv
1. Number of variables: 6

2. Number of cases/rows: 1704

3. Variable List:

- "country" 
    - Full name: Country 
    - Description: Name of the country 
    - Type of variable: Categorical
    - Unit of measurement: N/A 
    - Number of missing values: 0

- "year" 
    - Full name: Year
    - Description: Year of the observation
    - Type of variable: Integer
    - Unit of measurement: year
    - Number of missing values: 0

- "pop"
    - Full name: Population
    - Description: Population of the country in the given year
    - Type of variable: Numeric
    - Unit of measurement: people
    - Number of missing values: 0

-"continent"
    - Full name: Continent
    - Description: Continent where the country is located
    - Type of variable: Categorical
    - Unit of measurement: N/A
    - Number of missing values: 0

- "lifeExp"
    - Full name: Life Expectancy
    - Description: Average life expectancy at birth in years
    - Type of variable: Numeric
    - Unit of measurement: years
    - Number of missing values: 0

- "gdpPercap"
    - Full name: GDP per Capita
    - Description: Gross Domestic Product per capita in US dollars
    - Type of variable: Numeric
    - Unit of measurement: USD
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 82 KB

## 4.2 Vector data

### 4.2.1 delft-boundary.shp
1. Number of variables: 2

2. Number of cases/rows: 1

3. Variable List:
- "osm_id"
    - Full name: OSM ID
    - Description: Unique identifier for the OpenStreetMap feature
    - Type of variable: Integer
    - Unit of measurement: N/A
    - Number of missing values: 0

- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the boundary of Delft
    - Type of variable: Geometry (Polygon)
    - CRS: WGS 84
    - Number of missing values: 0


4. Specialised formats or other abbreviations used: N/A

5. Total file size: 26 KB (including all associated files)

### 4.2.2 delft-leisure.shp
1. Number of variables: 3

2. Number of cases/rows: 298

3. Variable List:
- "osm_id"
    - Full name: OSM ID
    - Description: Unique identifier for the OpenStreetMap feature
    - Type of variable: Integer
    - Unit of measurement: N/A
    - Number of missing values: 0

- "leisure"
    - Full name: Leisure Type
    - Description: Type of leisure facility (e.g., park, playground)
    - Type of variable: Categorical
    - Unit of measurement: N/A
    - Number of missing values: 26

- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the leisure facilities in Delft
    - Type of variable: Geometry (Point)
    - CRS: EPSG:28992
    - Number of missing values: 0   

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 166 KB (including all associated files)

### 4.2.3 delft-streets.shp
1. Number of variables: 3

2. Number of cases/rows: 11244

3. Variable List:
- "osm_id"
    - Full name: OSM ID
    - Description: Unique identifier for the OpenStreetMap feature
    - Type of variable: Integer
    - Unit of measurement: N/A
    - Number of missing values: 0   

- "highway"
    - Full name: Highway Type
    - Description: Type of highway (e.g., residential, primary)
    - Type of variable: Categorical
    - Unit of measurement: N/A
    - Number of missing values: 8

- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the street network in Delft
    - Type of variable: Geometry (Line)
    - CRS: EPSG:28992
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 7 074 KB (including all associated files)

### 4.2.4 nl-gemeenten.shp
1. Number of variables: 7

2. Number of cases/rows: 344

3. Variable List:
- "identifica"
    - Full name: Identificatie
    - Description: Full municipality code
    - Type of variable: string
    - Unit of measurement: N/A
    - Number of missing values: 0

- "naam"
    - Full name: Naam
    - Description: Name of the municipality
    - Type of variable: string
    - Unit of measurement: N/A
    - Number of missing values: 0

- "code"
    - Full name: Code
    - Description: Unique code for the municipality
    - Type of variable: string
    - Unit of measurement: N/A
    - Number of missing values: 0


- "ligtInProv"
    - Full name: Ligt in Provincie
    - Description: Province code in which the municipality is located
    - Type of variable: integer
    - Unit of measurement: N/A
    - Number of missing values: 0

- "ligtInPr_1"
    - Full name: Ligt in Provincie 1
    - Description: Province name in which the municipality is located
    - Type of variable: string
    - Unit of measurement: N/A
    - Number of missing values: 0

- "fuuid"
    - Full name: FUUID
    - Description: Unique identifier for the municipality
    - Type of variable: string
    - Unit of measurement: N/A
    - Number of missing values: 0

- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the municipality boundaries
    - Type of variable: Geometry (MultiPolygon)
    - CRS: EPSG:28992
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 11 435 KB (including all associated files)

### 4.2.5 nl-boundary.shp
1. Number of variables: 2

2. Number of cases/rows: 1

3. Variable List:
- "FID"
    - Full name: FID
    - Description: Feature ID, a unique identifier for the boundary feature
    - Type of variable: Integer
    - Unit of measurement: N/A
    - Number of missing values: 0

- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the boundary of the Netherlands
    - Type of variable: Geometry (MultiPolygon)
    - CRS: EPSG:28992
    - Number of missing values: 0


4. Specialised formats or other abbreviations used: N/A

5. Total file size: 587 KB (including all associated files)


### 4.2.6 bounding-box-brielle.shp
1. Number of variables: 1

2. Number of cases/rows: 1

3. Variable List:

- "query"
    - Full name: Query
    - Description: Query used to retrieve the bounding box
    - Type of variable: String
    - Unit of measurement: N/A
    - Number of missing values: 0

- "address"
    - Full name: Address
    - Description: Address of the bounding box location
    - Type of variable: String
    - Unit of measurement: N/A
    - Number of missing values: 0 

- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the bounding box of Brielle
    - Type of variable: Geometry (Polygon)
    - CRS: EPSG:28992
    - Number of missing values: 0   

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 11 KB (including all associated files)

### 4.2.7 data-brielle.shp
1. Number of variables: 1

2. Number of cases/rows: 0

3. Variable List:
- "geometry"
    - Full name: Geometry
    - Description: Geometric representation of the buildings in the Brielle area
    - Type of variable: Geometry (Polygon)
    - CRS: EPSG:28992
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 4 KB (including all associated files)

## 4.3 Raster data

### 4.3.1 tud-dsm-5m.tif
1. Number of variables (bands): 1

2. Number of cases/rows (pixels): 278692

3. Variable List (band names):
- "tud-dsm-5m"
    - Full name: Digital Surface Model (DSM) at 5m resolution
    - Description: Elevation data representing the surface of the TU Delft campus
    - Type of variable: Numeric
    - Unit of measurement: Meters
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 1 091 KB

### 4.3.2 tud-dtm-5m.tif
1. Number of variables (bands): 1

2. Number of cases/rows (pixels): 278692

3. Variable List (band names):
- "tud-dtm-5m"
    - Full name: Digital Terrain Model (DTM) at 5m resolution
    - Description: Elevation data representing the bare earth surface of the TU Delft campus
    - Type of variable: Numeric
    - Unit of measurement: Meters
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 1 091 KB

### 4.3.3 tud-dsm-5m-hill.tif
1. Number of variables (bands): 1

2. Number of cases/rows (pixels): 278692

3. Variable List (band names):
- "tud-dsm-5m-hill"
    - Full name: Hillshade of the Digital Surface Model (DSM) at 5m resolution
    - Description: Hillshade representation of the DSM to visualize terrain features
    - Type of variable: Numeric
    - Unit of measurement: Intensity of illumination ranging from 0 (darkest) to 255 (brightest)
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 274 KB

### 4.3.4 tud-dtm-5m-hill.tif
1. Number of variables (bands): 1

2. Number of cases/rows (pixels): 278692

3. Variable List (band names):
- "tud-dtm-5m-hill"
    - Full name: Hillshade of the Digital Terrain Model (DTM) at 5m resolution
    - Description: Hillshade representation of the DTM to visualize terrain features
    - Type of variable: Numeric
    - Unit of measurement: Intensity of illumination ranging from 0 (darkest) to 255 (brightest)
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 274 KB

### 4.3.5 tud-dtm-5m-hill-WGS84.tif
1. Number of variables (bands): 1

2. Number of cases/rows (pixels): 204360

3. Variable List (band names):
- "tud-dtm-5m-hill"
    - Full name: Hillshade of the Digital Terrain Model (DTM) at 5m resolution in WGS 84
    - Description: Hillshade representation of the DTM to visualize terrain features, projected in WGS
    - Type of variable: Numeric
    - Unit of measurement: Intensity of illumination ranging from 0 (darkest) to 255 (brightest)
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 730 KB

### 4.3.6 tudlib-rgb.tif
1. Number of variables (bands): 3

2. Number of cases/rows (pixels): 24271608

3. Variable List (band names):
- "tudlib-rgb_1"
    - Full name: Red band of the RGB composite
    - Description: Red channel of the RGB color composite for the TU Delft library area
    - Type of variable: Numeric
    - Unit of measurement: Intensity of color ranging from 0 (no intensity) to 255 (full intensity)
    - Number of missing values: 0

- "tudlib-rgb_2"
    - Full name: Green band of the RGB composite
    - Description: Green channel of the RGB color composite for the TU Delft library area
    - Type of variable: Numeric
    - Unit of measurement: Intensity of color ranging from 0 (no intensity) to 255 (full intensity)
    - Number of missing values: 0

- "tudlib-rgb_3"
    - Full name: Blue band of the RGB composite
    - Description: Blue channel of the RGB color composite for the TU Delft library area
    - Type of variable: Numeric
    - Unit of measurement: Intensity of color ranging from 0 (no intensity) to 255 (full intensity)
    - Number of missing values: 0

4. Specialised formats or other abbreviations used: N/A

5. Total file size: 71 138 KB

# 5. SHARING/ACCESS INFORMATION
## 5.1 Licenses/restrictions placed on the data:
The Geospatial Data Carpentry for Urbanism data is made available under the
ODbL 1.0 license, as it is derived from:
- OpenStreetMap data licensed under the ODbL 1.0 license
- Gapminder data licensed under the CC BY 4.0 license
- AHN data licensed under the CC0 1.0 license
- Luchfoto data licensed under the CC BY 4.0 license
- Bestuurlijke Gebieden (obtained from PDOK.nl) licensed under the CC BY 4.0 license

## 5.2 Links to other resources:

### 5.2.1 Links to other publicly accessible locations of the data: 

N/A

### 5.2.2 Links to publicly accessible scripts for analysis of the dataset:
- [Carpentry Repository](https://github.com/carpentries-incubator/r-geospatial-urban)

### 5.2.3 Was data derived from another source?
Yes, from the following sources:
- OpenStreetMap 
- Gapminder data
- AHN (Actueel Hoogtebestand Nederland)
- Luchtfoto (Aerial imagery of the Netherlands)
- PDOK (Publieke Dienstverlening Op de Kaart)

## 5.3 Recommended citation for this dataset:
Forgaci, C., Cottineau, C., Wilczynska, A., Petrovic, A., Cannatella, D.,
Urria Yáñez, I., San Millán Tejedor, J., Conceicao, J. F., Janssen, K.,
Garcia, M., Kubilay, S. (2024). Geospatial Data Carpentry for Urbanism Workshop
Data. Zenodo. 

This README.md file template was generated on 2022-04-19 by Claudiu Forgaci and Adele Therias according to the 4TU.ResearchData [Guidelines for creating a README file](https://data.4tu.nl/info/en/use/publish-cite/upload-your-data-in-our-data-repository) and the Cornell University template [Guide to writing "readme" style metadata](https://cornell.app.box.com/v/ReadmeTemplate) and is licensed under CC BY 4.0
