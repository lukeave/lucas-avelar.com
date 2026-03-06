---
_edit_last: "1"
_thumbnail_id: "368"
_yoast_wpseo_content_score: "30"
_yoast_wpseo_estimated-reading-time-minutes: "5"
_yoast_wpseo_primary_category: "1"
_yoast_wpseo_wordproof_timestamp: ""
author: avelar_adm
categories:
  - uncategorized
cover:
  alt: palladio logo
  image: /wp-content/uploads/2022/12/palladio-logo-e1678649892335.png
date: "2022-12-14T14:55:21+00:00"
guid: http://lucasavelar.org/?p=366
parent_post_id: null
post_id: "366"
title: 'Palladio: Everything is Connected'
url: /posts/palladio-everything-is-connected/

---
As surprising as it sounds, for a long time historians overlooked implicit connections between things, people, organizations, and ideas across time and space. But they were not unfamiliar to the idea of networks. As a crucial part of historical scholarship, historiographical works are fundamentally based on the premise that ideas, arguments, and scholars are somehow connected - even if they do not meet at the same time and space. Still, when writing histories of long processes, historians ignored complex networks that were hard to visualize.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-10.12.31-AM.png" alt="" caption="" >}}

Around the 1960s and 1970s, scholars influenced by the cultural and linguistic turn opposed the long-lasting traditional forms of writing history that prioritized orderly-chronological narratives and important political legacies. The negligence was a matter of contention between social historians who, although now looking at cultural practices and broadening their research questions to include a bottom-up perspective of history, still ignored less implicit connections that were shadowed in traditional forms of narrating time. Network analysis altered the landscape of historical studies for good.

Palladio is an integrated application that provides graphical visualization of data networks. As a product of the National Endowment for the Humanities Implementation Grant, it was developed for historians to think critically about their data, and as the website states, it is meant "for reflective practice." Like every tool discussed in this website, Palladio provides visualization and communication of historical data, but more importantly, it opens space for new questions and new arguments on the same information.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-10.21.56-AM.png" alt="" caption="" >}}

Although other formats of spreadsheet might work just as fine, CSV files are the recommended format to upload in Palladio. The application looks at columns and rows to generate a visual representation of the structured data with nodes (data points) and edges (connecting lines). Nodes can weighted in Palladio, but not edges. The spreadsheet [Dr. Doug Seefeldt](https://dougseefeldt.net/) provided us with had the authors of different books between 1850 and 1869 in column A and frequent terms associated with each author in column B. That means column A presented repetition while column B did not. When uploaded in entirety, the data looked like this:

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-10.38.47-AM.png" alt="" caption="" >}}

At first glance, one could feel the urge to throw their laptop at the wall. On a second glance, though, you might patiently recover and find it interesting to notice the connections between some of these authors through particular terms outside of the big, messy central web. For the sake of better visualizing those connections, I chose to weight the nodes representing the authors according to the frequency of terms and separate these nodes from each other as much as I could, resulting in a not-so-messy version of the network as you saw above.

Palladio's interactive interface is probably its greatest power. The user can interact with the nodes and reorganize the web in a way that visualizing particular edges becomes easier. Obviously, there are no good ways to avoid a messy center with so many terms associated with multiple authors, so this particular visualization is limited in what it can tell us.

But still, seeing how Domenech and Burton are connected, for example, is quite interesting. While the former brings up "nature," "human," and "soil," the latter mentions "church", "god," and "law," which puts their work in completely different subjects or fields. The word "world" seems to be one of the few connecting edge between the authors, which makes it a "weak tie."

Now, take a look at the connection between Coke and Townsend. According to the graph, the word "hour" is indeed the only connection between both authors. If we were to cut off those edges connecting Coke and Townsend to the word "hour," leaving the term fluctuating and disconnected from any author, we would have created a "structural hole." Structural holes are occupied by something or someone sitting at the intersection between individuals or other things that are otherwise disconnected without it.

Now, network visualizations can be bipartite and k-partite, and the one we experimented with was a bipartite graph. This means the visualization only supports two types of nodes, and they can only present connections between each type, never within one type. So authors do not have direct edges between themselves, only between authors and terms. The difference is on how the original data is structured, and if the questions we were asking the data were different, we would likely have to alter the very structure of the spreadsheet and how columns and rows are organized.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-11-09-at-1.42.05-PM.png" alt="" caption="" >}}

The visualization above helps to clarify what I mean. Instead of uploading the full data, I followed Dr. Seefeldt's suggestion of uploading just two authors worth of data. Coke and Bowles present at least 14 connecting terms between themselves. Since Palladio does not weight edges, it is hard to tell whether we are looking at weak ties. But the bipartite structure of the data makes it easy to see how authors are associated through the frequency of coinciding terms in their work - even if these authors never really connected between themselves in real life. This is the kind of implicit network connection historians can look at through network analysis. It puts aside traditionally chronological and place-based narratives that were rather limited by geographic boundaries and periodicity. The potential is huge.
