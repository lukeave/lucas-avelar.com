---
title: Communication Tools
showDate: false
showAuthor: false
showReadingTime: false
url: /communication-tools/

---
<style>
h1.post-title { display: none; }
</style>

<h1 style="text-align: center;">Digital Tools for Communication of Research Findings:</h1>

<h1 style="text-align: center;">Omeka and StoryMap</h1>

Between 2017 and 2019, I was a history interpreter and museum guide at the [Rio de Janeiro State Parliament's Tiradentes Palace](http://www.palaciotiradentes.rj.gov.br/). Since its inauguration in 1927, the building served as the national parliament when Rio de Janeiro was the federal district of Brazil. When the Culture Department asked me to contribute to the process of rewriting the history exhibits in the palace, the biggest challenge was to identify the best practices of curatorship and presentation of historical information for a vastly broad audience of daily visitors. One of the most frequent visiting groups was elementary and high school students who could have benefitted from experimenting with the process of curatorship itself. If I had any clue about digital tools back then, maybe that process would have been less challenging. In this page, I want to share my experiences with Omeka and ArcGIS StoryMap as digital tools that can improve presentation and communication of historical information. As I'm about to tell you, my experience with Omeka was not as successful as the opportunities I had to explore StoryMaps.

## Omeka

The great thing about Omeka is that it is an open-source system. The software is what we call a content management system (CMS), and the terminology is mostly self-explanatory: it increases the user's ability to manage and showcase digital contents in the form of a dynamic virtual exhibit. For what it offers to historians, museum professionals, and educators, the system is a powerful pedagogical tool.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-11-at-4.58.37-PM.png" alt="" caption="" >}}

The dashboard in Omeka is quite simple: it shows recently uploaded items and recently created collections to be showcased as virtual exhibits. First, the potential lies in its collaborative nature: multiple users can log into the system and contribute to the process of uploading, curating, managing, and showcasing digital objects like historical images. Second, it enables the user to curate each item with a consistent metadata schema.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-11-at-5.05.20-PM.png" alt="" caption="" >}}

The standards of the Dublin Core Metadata Element Set (DCMES) are widely accepted among resource management professionals. In this schema, each record has a set of elements or fields - here called properties - which include values that can be based on controlled vocabularies or not. Omeka allows the user to decide whether or not DCMES is the most appropriate metadata schema for each uploaded item, which is great to ensure broad accessibility and interoperability as [Metadata Librarian for Digital Collections Jessica L. Serrao](https://libraries.clemson.edu/our-organization/staff-directory/profile/?user=jserrao) informed our class during her talk.

When uploading an item to Omeka, the user is prompted to fill the record's metadata elements before making it publicly available as a digital exhibit. I have uploaded an aerial photograph of Clemson College in 1964 from the [Clemson University Photographs Digital Collection](https://digitalcollections.clemson.edu/explore/collections/ua100/) to Omeka to experiment with the tool.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-11-at-5.17.26-PM.png" alt="" caption="" >}}

When metadata is completed consistently, the item can be showcased in a new public page as part of the user's own digital exhibit, and it should look something like this:

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-11-at-5.32.10-PM.png" alt="" caption="" >}}

Since this was just a quick experiment, I couldn't explore other features of the system. But I'm confident that its power lies in the potential for collaboration between multiple users in creating and curating an exhibit from scratch. [Hallie Knipp](https://hallieknipp.net/) and I had ambitious ideas about how to experiment with this tool. Inspired by the spirit of Halloween, we went to [Clemson's Special Collections and Archives](https://libraries.clemson.edu/specialcollections/) located at the Strom Thurmond Institute to look for historical photographs of the campus during halloween across the years. The hope was to test Omeka's collaboration potential and create a digital exhibit on Clemson's Halloween traditions. Sadly, we didn't find much. And, of course, we were both too buried in work to move forward with the idea.

I can't help but wonder what all we could have done with Omeka when those elementary and high school students visited the Tiradentes Palace in Rio while curators and cultural managers were reimagining the exhibit. If every group had the opportunity to do a workshop using Omeka at the end of the visit and brainstorm ideas about new digital exhibits with particular focuses on the palace's history, we could have created the first interactive and fully collaborative public history project in the most important legislative museum of the country.

## ArcGIS StoryMaps

Professor [Elizabeth Tulanowski](https://watercenter.colostate.edu/view/water-experts-2/entry/3384/)'s introductory class on Geographic Information Systems at Colorado State University exposed me to ArcGIS tools. Developed by Esri, the world's leading supplier of GIS software and tools, ArcGIS tools are not open source. They are, however, available to most students and academics through institutional access. There are many open-source versions of ArcGIS Pro like ArcMap and QGIS, but it is true that the usability and advanced mapping functionalities of ArcGIS make it a preferable tool among GIS users and scholars working with spatial data. Like Omeka, ArcGIS StoryMap helps us visualize and present information to broad audiences. Differently from Omeka, it is not meant as a virtual exhibit of cultural resources, but rather a visual representation and place-based form of historical narrative.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-12-at-4.58.30-PM.png" alt="" caption="" >}}

In the summer of 2022, the [Geospatial Centroid at CSU](https://gis.colostate.edu/) hired me as an intern to work on a StoryMap project for the [Larimer County Department of Natural Resources](https://www.larimer.gov/naturalresources). I reviewed data from 1998 to 2022 and identified specific locations of projects that were awarded the County's [Small Grant for Community Partnering Program](https://www.larimer.gov/naturalresources/small-grants). After geolocating each of the awardees, I used ArcGIS StoryMap to create a place-based narrative about the twenty-five-year history of the program, and the different grant categories each project fell into ( [check out the full version of the storymap here](https://storymaps.arcgis.com/stories/d004f5b431b2475c807de7f67a14ed4a)).

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-12-at-6.03.41-PM.png" alt="" caption="" >}}

The screenshot above shows the basic layout of every story map: the textual information follows the visual component which is often an embedded Web Map or Web Application produced in ArcGIS Online. In the "side-by-side" layout, the viewer can either scroll through the text or interact with the Web Map. Above, you can see the Web Map includes a legend and showcases six different grant categories symbolized by different colors. But the story map creator can choose whether or not to show a particular layer of information for a specific slide of the story map.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-12-at-6.03.24-PM-1.png" alt="" caption="" >}}

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-12-at-6.02.40-PM-3.png" alt="" caption="" >}}

Here, the same Web Map was used to create an interactive Web Application in which the funding distribution and the population density were the relevant layers of information. In this stage of the story map, the user can expand the Web Application and interact with the different layers, either choosing to hide or visualize them. The overlap of different data provides significant insight into the criterion for awarding the Community Partnering Program Award throughout the county.

Historians benefit from locating history in space and having a visual understanding of spatial patterns across time. As a presentation and communication tool, ArcGIS StoryMaps goes beyond placing history: it provides a meaningful - and not necessarily chronological - narrative with embedded historical argument that benefits from multiple layers of information.

Want to share about a specific tool? Check out each tool’s blog post at the [Time Sensitive](/timesensitiveblog/).
