---
layout: page
title: "Building Inventory Visualizations"
permalink: /visualizations/
---

# Building Inventory Visualizations

This page showcases visualizations of the state building inventory.

## Visualization 1: Number of Buildings by Agency

<div id="vis1"></div>

## Visualization 2: Buildings by Congressional and Senate Districts

<div id="vis2"></div>

## Visualization 3: Square Footage of Buildings Over Years by Status

<div id="vis3"></div>

<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

<script>
  // Embed Visualization 1
  fetch('{{ site.baseurl }}/path/to/chart1.json')
    .then(response => response.json())
    .then(spec => vegaEmbed('#vis1', spec));

  // Embed Visualization 2
  fetch('{{ site.baseurl }}/path/to/chart2.json')
    .then(response => response.json())
    .then(spec => vegaEmbed('#vis2', spec));

  // Embed Visualization 3
  fetch('{{ site.baseurl }}/path/to/chart3.json')
    .then(response => response.json())
    .then(spec => vegaEmbed('#vis3', spec));
</script>
