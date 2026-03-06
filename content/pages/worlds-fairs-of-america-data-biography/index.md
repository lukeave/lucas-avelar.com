---
_edit_last: "1"
_wp_page_template: default
_yoast_wpseo_content_score: "30"
_yoast_wpseo_estimated-reading-time-minutes: "8"
_yoast_wpseo_wordproof_timestamp: ""
author: ""
date: ""
footnotes: ""
guid: http://lucasavelar.org/?page_id=632
parent_post_id: null
post_id: "632"
title: <strong>World’s Fairs of America Data Biography</strong>
showDate: false
showAuthor: false
showReadingTime: false
url: /worlds-fairs-of-america-data-biography/

---
**World’s Fairs of America** was created by Lucas Avelar. It is a spatial-historical dataset that contains information of seven different world’s fairs that took place in the United States in the late nineteenth and early twentieth centuries. Below is a data biography that details the dataset creation and its potential for usage by scholars and researchers that deal with inquiries of spatial nature.

#### Who made this dataset and why was it created?

Lucas Avelar gathered the historical data from archival documents and spatial data collection that resulted in this dataset as part of his Ph.D. dissertation project between 2023 and 2027. The data collection was part of a larger attempt to publicize a spatially oriented dataset and interactive web map applications of the most important world’s fairs that happened in the United States between 1876 and 1939. Each data file covers a different fair and provides information on the exhibit halls, monuments, and buildings, including their geolocation, measurements, and architectural style.

There is a total of seven data frames on seven world’s fairs. The larger research question that informed Avelar’s data collection was how the spatial organization of the fairs developed over time. He wanted to examine how the spatial narratives embedded in the events and their cultural landscapes reflected broader ideas of modernity and tradition, cultural hegemony, and national identity. By including information of multiple sites on the fairs’ grounds, pathways, and entrances, Avelar hoped to reconstruct the historical perspective of fair goers and how they perceived fair makers’ intended messages in the built environment.

#### What's in the data?

**World’s Fairs of America** contains seven data files for each of the following world’s fairs: the Centennial Exposition of 1876 (Philadelphia), the World’s Columbian Exposition of 1893 (Chicago), Louisiana Purchase Exposition of 1904 (St Louis), the Panama California Pacific Exposition of 1916 (San Diego), the Bronx International Exposition of Science, Arts, and Industries of 1918 (New York), the New York World’s Fair of 1939 (New York), and the Golden Gate International Exposition of 1939 (San Francisco). In each data frame, each record or observation represents information about a single building, pavilion, monument, statue, or exhibit hall in one of the above-mentioned fairs. Each data frame contains at least 14 fields or variables that are specified in the data dictionary for each file. Each data file has its associated data dictionary file. See the Louisiana Purchase Exhibition data dictionary below as an example:

{{< figure src="/wp-content/uploads/2023/03/Screenshot-2023-03-13-at-11.45.44-AM.png" alt="" caption="" >}}

#### How was the data created?

The **World’s Fairs of America** data was created in three stages: archival research, spatial data collection, and data processing and geolocation.

###### **Stage 1: Archival Research**

Over five years of data collection and archival research preceded the creation of this dataset. The main sources of information were the authentic guides for each of the examined fairs, in which the fair organizers recorded descriptive information about the pavilions, exhibit halls, statues, and foreign participants.

{{< figure src="/wp-content/uploads/2023/03/Screenshot-2023-03-13-at-11.58.42-AM.png" alt="" caption="" >}}

Avelar cross-referenced the information on the authentic guides and official publications by fair organizers with data from different sources, including newspapers, foreign reports, government records, minutes, floor plans, maps, and pictures. These and other documentation were gathered from institutions like the Library of Congress, the Chicago Public Library, the Missouri Historical Society, and the Queens Public Library.

Plenty of documents are also available through the Adam Matthew Digital Library. Avelar made the decision to transcribe potentially useful information into a draft-like spreadsheet before processing the data into the matrix spreadsheet. The draft spreadsheet contained information on where and how the records were archived – if physical or digital –, their material condition if applicable, and the hierarchical logic behind the archival storage of each record.

###### Stage 2: Spatial Data Collection

{{< figure src="/wp-content/uploads/2023/03/Picture1.png" alt="" caption="" >}}

To acquire information on signs of historic interpretation, continuities, and ruptures in the landscape between the years of the fair and the present time, Lucas Avelar went to the grounds where the fairs took place in Philadelphia, Chicago, St Louis, San Diego, New York, and San Francisco to collect spatial data using ArcMap and a GPS device. The data were then stored in spatial datasets that contained basic information on each collected data point, including latitude and longitude, visibility quality, access quality, and pictures taken on the field.

{{< figure src="/wp-content/uploads/2023/03/Screenshot-2023-03-14-at-8.24.22-AM.png" alt="" caption="" >}}

###### Stage 3: Data Processing and Geocoding

Before merging the spatial data sets with the matrix data, Avelar had to go through the third stage of data creation: geocoding the data gathered from archival research and data processing. Data processing takes different forms in different circumstances. Generally, it implies manipulation and conversion of the raw data into machine-readable form for the purpose of computational analysis. Avelar processed the data from the matrix dataset to create the different data files for each world’s fair, formatting the variables’ names, the observations, and the class of each variable to enable computing and manipulation.

The geocoding approach relied on RStudio programming language for sites with street address information. Using Google API and Geocoder, the R script retrieved latitude and longitude information for corresponding matches of street, city, and state. However, due to the temporary nature of most sites in this dataset, the code was not enough to retrieve most of the geocoordinates. Avelar then resorted to georeferencing historic maps of the fairs and overlay them with contemporary maps to determine the latitude and longitude of each record. The R code, script files, and georeferenced historic maps can be found in the [Github Repository for the World's Fairs of America data](https://github.com/lukeave).

Lastly, controlled vocabulary developed in AirTable was used to make the dataset tidy and keep consistency throughout the records.

#### How should I use this data?

```
library(ggmap)
library(ggplot2)
library(tidygeocoder)
library(tidyverse)

qmplot(latitude, longitude, data= stlouis.1904.data, maptype ="toner-background")
```

{{< figure src="/wp-content/uploads/2023/03/Screenshot-2023-03-14-at-8.19.13-AM.png" alt="" caption="" >}}

The map above shows some sites of the St Louis 1904 World’s Fair geopositioned through processing the CSV data file in R and using the ggmap library to plot the data points on a map based on latitude and longitude information. If you hope to make a visualization of one of the world’s fairs, keep in mind that the geocoding process and georeferencing of the fairs’ historic maps present limitations since sites rarely possess street addresses. Further, maps were meant to guide visitors through the fair grounds and in no way provided accurate geolocation of exhibits. Still, visualizing the estimated location and spatial organization of the fair sites can provide scholars with potentially new research questions about the relationship between space production and narratives of modernity and cultural identities.

```
#Load ggmap and ggplot2 libraries
library(ggmap)
library(ggplot2)
#Plot the cost for each category
ggplot(data=stlouis.1904.data, mapping= aes(x = category, y = cost, color = category)) +
  geom_col()

# Install the GGally package, an extension for ggplot, and load the GGally library.
install.packages("GGally")
library(GGally)
# Plot the correlation between cost and area for each category
ggparcoord(stlouis.1904.data,
           columns = 7:8, groupColumn = 4,
           scale="uniminmax",
           showPoints = TRUE,
           title = "Correlation: Area and Cost",
           alphaLines = 0.3
)
```

{{< figure src="/wp-content/uploads/2023/03/Screenshot-2023-03-14-at-8.17.18-AM.png" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2023/03/Screenshot-2023-03-14-at-8.17.32-AM.png" alt="" caption="" >}}

Data manipulation and analysis can provide meaningful insights in many different directions for each of the world’s fairs. In the examples above, we can visualize correlation between cost and area for each site according to their categorization (i.e., state, foreign, territory) and easily determine the priority when it comes to expenses for each type of construction.

Since each CSV file contains a large number of observations and the variables are not precisely the same for every fair, it is recommended that the user exercise caution when doing quantitative analysis. For qualitative purposes, the data is useful in comparative analysis of each fair’s spatial arrangement. For instance, we might want to ask a question such as: how far away was the Philippine Exhibit from the main entrance of the fair? What were the intended paths that visitors were expected to take to reach said exhibit? And what other sites would they see on the way before seeing the Philippine Exhibit? What type of access was provided to reach said grounds?

And more broadly, what does all of this tell us about the production of space and ideologies of modernity, tradition, and national identity?
