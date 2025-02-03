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
{% for page in redirects %}| {{ page.title | escape }} | {{ page.description | escape }} | [{{ page.url }}]({{ page.url | relative_url }}) | <{{ page.embed_url }}> |{% endfor %}


{% for page in redirects %}
- [{{ page.url }}]({{ page.url | relative_url }}) 🔀 <{{ page.embed_url }}> ➡️ {{ page.title | escape }} - {{ page.description | escape }}
{% endfor %}

## Other Apps

Biodiversity Pathways:

- Moose app for Biodiversity Pathways: <https://psolymos.shinyapps.io/moose/>
- BC Caribou prioritization tool: <https://biodiversity-pathways.shinyapps.io/bcprioritytool/>
- WildLift: <https://abbiodiversity.shinyapps.io/WildLift/>

Western Boreal Initiatives - trees & birds:

- Full extent: <https://wbi.predictiveecology.org/apps/wbi/>
- Northwest Territories: <https://wbi.predictiveecology.org/apps/nwt/>

Statistics/teaching:

- Data cloning apps for teaching statistics: <https://psolymos.shinyapps.io/dcapps/>

Environmental data:

- Air monitoring data explorer with kriging: <https://psolymos.shinyapps.io/airquality/>
- Interactive air data explorer: <https://analythium.shinyapps.io/airglider/>
- SO2 map with autoplay (spatial time series): <https://analythium.shinyapps.io/so2-map/>

Alberta Tier 1 3D plot:

- <https://analythium.shinyapps.io/plot3d/>

COVID dashboards:

- <https://hub.analythium.io/covidapp/>
- <https://analythium.shinyapps.io/covid-19-abmap/>
- <https://analythium.shinyapps.io/covid-19-alberta/>

Other:

- Red Deer River chemistry monitoring: <https://analythium.shinyapps.io/reddeer/>
