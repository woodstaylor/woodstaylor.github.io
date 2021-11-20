---
title: "visualizing hierarchies in R"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - infographics
  - science
---

Here are a couple ways of exploring hierarchical (nested) data in R. This dataset consisted of taxonomic (order, family, genus, species) data for dragonflies and damselflies. I wanted to visualize the representation of species in the dataset across biological levels.

<p align="center">
<img src="/assets/infographics/taxonomy_circlepack.jpg" alt="circlepack"/>
</p>

^ This first approach used a [circle pack diagram](https://www.r-graph-gallery.com/circle-packing.html). The circle size represents the number of species per level, with the finest resolution being genera (filled blue cirles). This was realitively easy to code with the [igraph package](https://github.com/igraph/rigraph). But I wanted to also show species attributes on the graph (e.g., relative differences in body size among species).

<p align="center">
<img src="/assets/infographics/taxonomySum.jpg" alt="pictograph"/>
</p>

^ To do this, I wanted to use a [pictogram chart](https://dataforvisualization.com/charts/pictogram-chart/https://dataforvisualization.com/charts/pictogram-chart/).  

This was a bit harder to do in R. The [waffle package](https://github.com/hrbrmstr/waffle) does this well. But I wanted to customize species positions. So I determined 'coordinates' (x & y locations) of orders/families/species based on an imaginary grid (here the grid was 7 x 15) and used the [ggimage package](https://github.com/GuangchuangYu/ggimage) to display icons for each species. 

