---
_edit_last: "1"
_thumbnail_id: "455"
_yoast_wpseo_content_score: "30"
_yoast_wpseo_estimated-reading-time-minutes: "4"
_yoast_wpseo_primary_category: "1"
_yoast_wpseo_wordproof_timestamp: ""
author: Lucas Avelar
cover:
  alt: tableau
  image: /wp-content/uploads/2022/12/tableau.png
date: "2022-12-14T20:04:12+00:00"
guid: http://lucasavelar.org/?p=453
parent_post_id: null
post_id: "453"
title: 'Tableau: Inquiring Far and Beyond with Data Visualization'
url: /posts/tableau-inquiring-far-and-beyond-with-data-visualization/

---
To experiment with Tableau, an interactive data visualization application, I acquired data in XLSX format from the [National Register of Historic Places](https://www.nps.gov/subjects/nationalregister/database-research.htm) online database. The spreadsheet contained information on all the properties listed in the National Register until 2022 for local, state, national, and international significance. It also displayed geographic information with street addresses, cities, counties, and states for each of the property.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-11.41.46-AM.png" alt="" caption="" >}}

Tableau is highly sophisticated, and I would need much more extra time and training to figure out how to properly create visualizations out of large datasets like the NRHP data. Knowing that I could not break the software or the dataset, I tried some things out. Here is what I could come up with:

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-2.16.16-PM.png" alt="" caption="" >}}

This took me some hours of troubleshooting as I still do not master the ways of Tableau in structuring the data to make it a good fit for each graph. What this visualization tells is is where in the country each category of historic place is most concentrated, and which states have more properties listed for national significance. With the street address data, Tableau was able to generate longitude and latitude data for each of the listed properties.

The first column "National Level" is the indicator whether or not national significance was assigned to each property displayed on the map. This means that the first row, "False," only shows properties with no national significance while the second row, "True," represents the ones that have it. I tried to symbolize each category (building, district, object, site, and structure) with different colors and weight the data points on the map according to the concentration of listed properties in the same area.

Because of this choice of symbology and the way the data is structured in this visualization, we can tell, for example, that there are more buildings that sites listed; that the northeast and east coast concentrate the majority of historic places in the National Register; and that there are more local- and state-level significant properties listed than nationally significant properties across the United States.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-2.48.17-PM.png" alt="" caption="" >}}

Here, I experimented a different form of visualizing the data and chose to include information on Federal Agencies associated with the properties listed in the National Register. There are many ways to look at this information, but I choose to be creative and play with geolocation. The _x_ axe shows the latitude and the _y_ axe shows longitude of each listed property, making the position of each data point in a field significant for the analysis. The visualization tells us that the Forest Service and the Coast Guard, at least among those five agencies displayed in the screenshot, have significant association with historic sites of the National Register.

The potential to experiment with Tableau seems infinite. During seminar, [Dr. Matt Chambers](https://www.tableau.com/about/blog/contributors/matt-chambers) spoke to us about how he used the software to create amazing visualizations about the history of the NFL. Chambers is the Executive Director of Visual Analytics at Clemson CCIT and has some fun stuff going on in Tableau. Check out his public visualizations to see more of what this powerful software can do.

Working with a historical dataset like the NRHP, I hoped to understand how historians can take advantage of Tableau for visualizing data. But there is so much going on that it can be overwhelming. It does prove the point that visualizations are meant for inspire new research questions and different arguments, not simply to communicate the findings of a previous inquiry.
