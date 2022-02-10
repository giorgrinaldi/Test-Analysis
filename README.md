# Test Analysis

In recent years, social media activity from influential people
has proven to have very serious real-world repercussions.
Elon Musk, the eclectic personality at the head of innovative enterprises like SpaceX and Tesla, exemplifies this phenomenon. His tweets have notoriously been able to significantly influence the value of financial assets like Bitcoin (Browne, 2021) and (perhaps more importantly for him) the value of his own company’s stock.
Consequently, there is great interest in understanding the ways in which Musk’s Twitter
activity affects Tesla’s stock. A system capable of accurately predicting the relation between these two things could prove to be useful for multiple different stakeholders, both internal and external to the company. Musk himself, for instance, could utilize such an application to determine if a tweet is worth posting or perhaps to tweak their wording so as to maximize their positive effects (or minimize their negative effects) on stock value. This paper describes our approach to building such an application by programming a supervised machine learning algorithm.

First of all, it has to be noted that in order to understand the impact of Musk’s Twitter
posts on Tesla’s share price, we decided not to use the type of sentiment analysis introduced in
the tutorials but instead to apply the “term frequency–inverse document frequency” (tf-idf)
approach which determines how important certain words are in a collection of documents.
Generally speaking, the tf-idf is composed of two statistics, namely the term frequency (TF) and
Inverse document frequency (IDF). The TF determines the weight of a term in a document, i.e
the number of times a certain word appears in a document. The IDF determines the specificity of
a term and “can be quantified as an inverse function of the number of documents in which it
occurs”. The intuition behind the IDF is that a certain word which is contained in multiple
documents should be given less weight than one which only appears in a small number of
documents (Robertson, 2004).
