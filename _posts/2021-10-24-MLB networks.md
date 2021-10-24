---
title: "Network analysis: MLB"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - infographics
  - sports
---
<p align="center">
<img src="/assets/infographics/MLBnetworks.jpg" alt="population"/>
</p>

Here, I explore basic components of social networks using [Sean Lahman's MLB dataset](http://www.seanlahman.com/baseball-archive/statistics/). The infographic displays **centrality** of teams based on relationships of players shared. Those teams with higher centrality share more players with other teams, indicating importance to the MLB team network. I also used the overall network to identify **clusters** based on centrality. This revealed a cluster of highly central teams (e.g., STL - Cardinals, CIN - Reds, CHC - Cubs) and teams with low centrality (e.g., COL - Rockies, KC - Royals). Those teams in cluster 1 share more player connections with other teams than those in cluster 2, indicating their importance to the MLB network.

I also showed player-manager networks within teams (based on the number of years associated with the same team together) in this interactive graphic: [MLB player-manager networks](https://woodstaylor.shinyapps.io/MLBmanagerNetworks/).

You can download this visualization here: [Download here](https://github.com/woodstaylor/woodstaylor.github.io/raw/master/assets/infographics/MLBnetworks.pdf).

