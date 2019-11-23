---
title: "Understanding the Global Arms Trade Network: Analysis of Different Community Detection Methods"
collection: research
type: "Research"
permalink: /research/network
venue: "Network Science Capstone Group Research Project, April - May, 2019"
date: 2019-04-02
location: "Saint Paul, Minnesota"
---

[This project](https://www.dropbox.com/s/hori04hc3f7e4bo/Network%20Science.pdf?dl=0) is a social network visualization and analysis on global arms trade using arms trade data from the Stockholm International Peace Research Institute database from 2016 - 2018. I constructed the social network and detect hidden community within this network using the state-of-the-art Louvain algorithm. Later, I used hierarchical clustering to consider the node attributes of each country, such as their domestic arms production, freedom score and membership of international peace treaties. We also incorporate countries location to see if, for example, European countries are "European" in terms of arms trade. In the end, I combined the topological structure and node attributes to generate a more comprehensive community detection algorithms. We found that powerful countries tend to ally themselves with each others and leave countries with less military capacity in another community.

Below are some cool visualizations:

<img src="/images/network.png" width="620" height="610" alt="Modularity Network">

<img src="/images/MSTnetwork.png" width="620" height="315" alt="Joint Clustering">

Figure 2: Node Attributes with locations, arms production, and freedom scores. The layout corresponds to geographical locations of countries' capital.
