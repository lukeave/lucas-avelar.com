---
title: Visualization Tools
showDate: false
showAuthor: false
showReadingTime: false
url: /visualization-tools/

---

<style>
h1.post-title { display: none; }
</style>

<h1 style="text-align: center;">Digital Tools for Data Visualization:</h1>

<h1 style="text-align: center;">Voyant, Palladio, and Tableau</h1>

Presentation of research findings is just as important as the analysis itself. If you haven't checked out the Communication Tools page in this website, give it a shot before moving forward. Communication of historical knowledge is indeed important, and the tools I discussed in the previous page can sure help with that. Some digital tools for data visualization, however, go beyond presentation. They enable further inquiry, new answers, and more in-depth analysis of the same data. Voyant, Palladio, and Tableau are examples of visualization tools that are rather crucial for new historical interpretations.

## Voyant

When [Dr. Leisl Carr Childers](https://leislcarrchilders.org/) introduced me to [Voyant](https://voyant-tools.org/) during her graduate methods seminar at Colorado State University, I realized a few things. First, that historians can take for granted the textual nature of traditional primary sources. The structure, vocabulary, and terms of a corpus tell us a lot about culture and society and even change over time. Second, that the process of text mining, so dear to digital humanists and linguistics scholars, can prove invaluable for historical analysis. Transforming text into structured data suitable for computational processes opens a new venue of interpretation of historical documents and argumentation.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-13-at-12.12.44-PM.png" alt="" caption="" >}}

Voyant allows the user to upload a corpus of text directly into the home page. In the process of text mining, the tool recognizes terms in the uploaded corpus that are likely stop words and therefore irrelevant for analysis, like "the" and "a." The result is a set of at least five different visualizations (or "skins") that provide different insights into the examined corpus. For the sake of this experiment, I have uploaded the corpus of Frankenstein by Mary Shelley.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-13-at-11.16.49-PM.png" alt="" caption="" >}}

The skin _Term_ s is arguably the most straight forward. It displays the count of each term of the corpus and allows the user to decide whether or not they should edit the stop-word list for the sake of the research question. I have removed words like "I" and "shall" to have a better grasp of most frequent terms with semantic value.

In the skin _Reader_, you may notice I have searched for "mind\*" and "heart\*" to assess the distribution of these terms and their variations (represented here by the command "\*") throughout the corpus. My hope was to experiment with the tool's analytical potential and see where, in the corpus, the terms showed up more. In this sense, I was looking at frequency - the number of times the phrase appears in a corpus - and concordance - the context in which it does - at the same time through the _Reader_ skin, two important concepts in text analysis and the field of linguistics. The _Trends_ skin provides an even better sense of frequency, but barely touches on concordance and contextual placement. See below.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-9.28.19-AM.png" alt="" caption="" >}}

Now, the power of examining concordance and correlations of terms - or "types" - throughout a large corpus is the gem of text mining for digital historians. Humanistic inquiry generally requires qualitative thinking, but text analysis, as Stefan Sinclair and Geoffrey Rockwell suggest, is a symbiosis between quantitative and qualitative operations.[^1] In a text, words can represent the subject or the object of humanistic processes, holding on to different levels of agency according to their positionality. When historians interpret textual documents as data and pay attention to things like concordance and collocation - the level of variation of concordance of a type - they can draw innovative arguments about the past, chronological patterns, and cultural and social change over time.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-9.44.29-AM.png" alt="" caption="" >}}

Above, the _Correlations_ skin shows how qualitative and quantitative thinking merge in text mining. The Correlation coefficient (r) indicates how the frequencies of term 1 and term 2 are related throughout the corpus. When closer to 1, (r) suggests the frequencies either rise or fall together. When closer to -1, (r) indicates inverse correlation: when one frequency rises, the other falls.

## Palladio

As surprising as it sounds, for a long time historians overlooked implicit connections between things, people, organizations, and ideas across time and space. But they were not unfamiliar to the idea of networks. As a crucial part of historical scholarship, historiographical works are fundamentally based on the premise that ideas, arguments, and scholars are somehow connected - even if they do not meet at the same time and space. Still, when writing histories of long processes, historians ignored complex networks that were hard to visualize.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-10.12.31-AM.png" alt="" caption="" >}}

Around the 1960s and 1970s, scholars influenced by the cultural and linguistic turn opposed the long-lasting traditional forms of writing history that prioritized orderly-chronological narratives and important political legacies. The negligence was a matter of contention between social historians who, although now looking at cultural practices and broadening their research questions to include a bottom-up perspective of history, still ignored less implicit connections that were shadowed in traditional forms of narrating time. Network analysis altered the landscape of historical studies for good.

Palladio is an integrated application that provides graphical visualization of data networks. As a product of the National Endowment for the Humanities Implementation Grant, it was developed for historians to think critically about their data, and as the website states, it is meant "for reflective practice." Like every tool discussed in this website, Palladio provides visualization and communication of historical data, but more importantly, it opens space for new questions and new arguments on the same information.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-10.21.56-AM.png" alt="" caption="" >}}

Although other formats of spreadsheet might work just as fine, CSV files are the recommended format to upload in Palladio. The application looks at the data variables and observations to generate a visual representation of the structured data with nodes (data points) and edges (connecting lines). Nodes can be weighted in Palladio, but not edges. The spreadsheet [Dr. Doug Seefeldt](https://dougseefeldt.net/) provided us with to experiment with the tool during seminar had simply two variables: the authors of different books between 1850 and 1869 in column A and frequent terms associated with each author in column B. That means column A presented repetition while column B did not. When uploaded in entirety, the data looked like this:

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-10.38.47-AM.png" alt="" caption="" >}}

At first glance, one could feel the urge to throw their laptop at the wall. On a second glance, though, you might patiently recover and find it interesting to notice the connections between some of these authors through particular terms outside of the big, messy central web. For the sake of better visualizing those connections, I chose to weight the nodes representing the authors according to the frequency of terms and separate these nodes from each other as much as I could, resulting in a not-so-messy version of the network as you saw above.

Palladio's interactive interface is probably its greatest power. The user can interact with the nodes and reorganize the web in a way that visualizing particular edges becomes easier. Obviously, there are no good ways to avoid a messy center with so many terms associated with multiple authors, so this particular visualization is limited in what it can tell us.

But still, seeing how Domenech and Burton are connected, for example, is quite interesting. While the former brings up "nature," "human," and "soil," the latter mentions "church", "god," and "law," which puts their work in completely different subjects or fields. The word "world" seems to be one of the few connecting edges between the authors, which makes it what we call a "weak tie."

Now, take a look at the connection between Coke and Townsend. According to the graph, the word "hour" is indeed the only connection between both authors. If we were to cut off those edges connecting Coke and Townsend to the word "hour," leaving the term fluctuating and disconnected from any author, we would have created a "structural hole." Structural holes are occupied by something or someone sitting at the intersection between individuals or other things that are otherwise disconnected without it.

Now, network visualizations can be bipartite and k-partite, and the one we experimented with was a bipartite graph. This means the visualization only supports two types of nodes, and they can only present connections between each type, never within one type. So authors do not have direct edges between themselves, only between authors and terms. The difference is in how the original data is structured, and if the questions we were asking the data were different, we would likely have to alter the very structure of the spreadsheet and how variables and observations are organized. We would likely have to widen the dataset, which means increasing the number of variables (the columns) and reducing the number of observations (the rows), avoiding repetition in the first column with the authors names. But that is a conversation for another time.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-11-09-at-1.42.05-PM.png" alt="" caption="" >}}

The visualization above helps to clarify what I mean. Instead of uploading the full data, I followed Dr. Seefeldt's suggestion of uploading just two authors worth of data. Coke and Bowles present at least 14 connecting terms between themselves. Since Palladio does not weight edges, it is hard to tell whether we are looking at weak ties. But the bipartite structure of the data makes it easy to see how authors are associated through the frequency of coinciding terms in their work - even if these authors never really connected between themselves in real life. This is the kind of implicit network connection historians can look at through network analysis. It puts aside traditionally chronological and place-based narratives that were rather limited by geographic boundaries and periodicity. The potential is huge.

## Tableau

To experiment with Tableau, an interactive data visualization application, I acquired data in XLSX format from the [National Register of Historic Places](https://www.nps.gov/subjects/nationalregister/database-research.htm) online database. The spreadsheet contained information on all the properties listed in the National Register until 2022 for local, state, national, and international significance. It also displayed geographic information with street addresses, cities, counties, and states for each of the properties.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-11.41.46-AM.png" alt="" caption="" >}}

Tableau is highly sophisticated, and I would need much more extra time and training to figure out how to properly create visualizations out of large datasets like the NRHP data. Knowing that I could not break the software or the dataset, I tried some things out. Here is what I could come up with:

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-2.16.16-PM.png" alt="" caption="" >}}

This took me some hours of troubleshooting as I still do not master the ways of Tableau in structuring the data to make it a good fit for each graph. What this visualization tells us is where in the country each category of historic place is most concentrated, and which states have more properties listed for national significance. With the street address data, Tableau was able to generate longitude and latitude coordinates for each of the listed properties.

The first column "National Level" is the indicator whether or not national significance was assigned to each property displayed on the map. This means that the first row, "False," only shows properties with no national significance while the second row, "True," represents the ones that have it. I tried to symbolize each category (building, district, object, site, and structure) with different colors and weight the data points on the map according to the concentration of listed properties in the same area.

Because of this choice of symbology and the way the data is structured in this visualization, we can tell, for example, that there are more buildings that sites listed; that the northeast and east coast concentrate the majority of historic places in the National Register; and that there are more local- and state-level significant properties listed than nationally significant properties across the United States.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-2.48.17-PM.png" alt="" caption="" >}}

Here, I experimented a different form of visualizing the data and chose to include information on Federal Agencies associated with the properties listed in the National Register. There are many ways to look at this information, but I choose to be creative and play with geolocation. The _x_ axe shows the latitude and the _y_ axe shows longitude of each listed property, making the position of each data point in a field significant for the analysis. The visualization tells us that the Forest Service and the Coast Guard, at least among those five agencies displayed in the screenshot, have significant association with historic sites of the National Register.

The potential to experiment with Tableau seems infinite. During seminar, [Dr. Matt Chambers](https://www.tableau.com/about/blog/contributors/matt-chambers) spoke to us about how he used the software to create amazing visualizations about the history of the NFL. Chambers is the Executive Director of Visual Analytics at Clemson CCIT and has some fun stuff going on in Tableau. Check out his public visualizations to see more of what this powerful software can do.

Working with a historical dataset like the NRHP data, I hoped to understand how historians can take advantage of Tableau for visualizing data. But there is so much going on that it can be overwhelming. It does prove the point that visualizations are meant to inspire new research questions and different arguments, not simply to communicate the findings of a previous inquiry.

Want to share about a specific tool? Check out each tool’s blog post at the [Time Sensitive](/timesensitiveblog/).

* * *

[^1]: Stéfan Sinclair and Geoffrey Rockwell, “Text Analysis and Visualization: Making Meaning Count,” in <em>A New Companion to Digital Humanities</em>, ed. Susan Schreibman et. al. (John Wiley &amp; Sons, Ltd, 2016).
