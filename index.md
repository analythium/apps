---
title: Apps
description: A list of apps
layout: list
---

# Apps

## Embedded Apps

{% assign redirects = site.pages | where_exp: "item", "item.embed_url != nil" %}
| Title      | Description | Embed URL    | Original URL    |
|------------|-------------|--------------|-----------------|
{% for page in redirects %}| {{ page.title | escape }} | {{ page.description | escape }} | [{{ page.url }}]({{ page.url | relative_url }}) | <{{ page.embed_url }}> |
{% endfor %}

## Other Apps (not embedded)

Western Boreal Initiatives - trees & birds:

- Full extent: <https://wbi.predictiveecology.org/apps/wbi/>
- Northwest Territories: <https://wbi.predictiveecology.org/apps/nwt/>

COVID dashboards:

- <https://hub.analythium.io/covidapp/>
- <https://analythium.shinyapps.io/covid-19-abmap/>
- <https://analythium.shinyapps.io/covid-19-alberta/>

