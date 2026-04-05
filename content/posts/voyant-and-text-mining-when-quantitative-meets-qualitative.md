---
author: Lucas Avelar
cover:
  alt: voyant
  image: /wp-content/uploads/2022/12/voyant.png
date: "2022-12-14T14:53:30+00:00"
title: 'Voyant and Text Mining: When Quantitative Meets Qualitative'
url: /posts/voyant-and-text-mining-when-quantitative-meets-qualitative/

---
When [Dr. Leisl Carr Childers](https://leislcarrchilders.org/) introduced me to [Voyant](https://voyant-tools.org/) during her graduate methods seminar at Colorado State University, I realized a few things. First, that historians can take for granted the textual nature of traditional primary sources. The structure, vocabulary, and terms of a textual corpus tell us a lot about culture and society and even change over time. Second, that the process of text mining, so dear to digital humanists and linguistics scholars, can prove invaluable for historical analysis. Transforming text into structured data suitable for computational processes opens a new venue of interpretation of historical documents and argumentation.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-13-at-12.12.44-PM.png" alt="" caption="" >}}

Voyant allows the user to upload a corpus of text directly into the home page. In the process of text mining, the tool recognizes terms in the uploaded corpus that are likely stop words and therefore irrelevant for analysis, like "the" and "a." The result is a set of at least five different visualizations (or "skins") that provide different insights into the examined corpus. For the sake of this experiment, I have uploaded the corpus of Frankenstein by Mary Shelley.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-13-at-11.16.49-PM.png" alt="" caption="" >}}

The skin _Term_ s is arguably the most straight forward. It displays the count of each term of the corpus and allows the user to decide whether or not they should edit the stop-word list for the sake of the research question. I have removed words like "I" and "shall" to have a better grasp of most frequent terms with semantic value.

In the skin _Reader_, you may notice I have searched for "mind\*" and "heart\*" to assess the distribution of these terms and their variations (represented here by the command "\*") throughout the corpus. My hope was to experiment with the tool's analytical potential and see where, in the corpus, the the terms showed up more. In this sense, I was looking at frequency - the number of times the phrase appears in a corpus - and concordance - the context in which it does - at the same time through the _Reader_ skin, two important concepts in text analysis and the field of linguistics. The _Trends_ skin provides an even better sense of frequency, but barely touches on concordance and contextual placement. See below.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-9.28.19-AM.png" alt="" caption="" >}}

Now, the power of examining concordance and correlations of terms - or "types" - throughout a large corpus is the gem of text mining for digital historians. Humanistic inquiry generally requires qualitative thinking, but text analysis, as Stefan Sinclair and Geoffrey Rockwell suggest, a symbiosis between quantitative and qualitative operations. In a text, words can represent the subject or the object of humanistic processes, holding on to different levels of agency according to their positionality. When historians interpret textual documents as data and pay attention on things like concordance and collocation - the level of variation of concordance of a type - they can draw innovative arguments about the past, chronological patterns, and cultural and social change over time.

{{< figure src="/wp-content/uploads/2022/12/Screenshot-2022-12-14-at-9.44.29-AM.png" alt="" caption="" >}}

Above, the _Correlations_ skin shows how qualitative and quantitative thinking merge in text mining. The Correlation coefficient (r) indicates how the frequencies of term 1 and term 2 are related throughout the corpus. When closer to 1, (r) suggests the frequencies either rise or fall together. When closer to -1, (r) indicates inverse correlation: when one frequency rises, the other falls.
