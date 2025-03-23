---
title: Apps
description: A list of apps
layout: list
---

# Apps

These apps were developed by [Analythum](https://a8m.io)

## Embedded Apps

{% assign redirects = site.pages | where_exp: "item", "item.embed_url != nil" %}
| Title      | Description | Embed URL    | Original URL    |
|------------|-------------|--------------|-----------------|
{% for page in redirects %}| {{ page.title | escape }} | {{ page.description | escape }} | [{{ page.url }}]({{ page.url | relative_url }}) | <{{ page.embed_url }}> |
{% endfor %}

## Other Apps (not embedded)

- Western Boreal Initiative, full extent: <https://wbi.predictiveecology.org/apps/wbi/>
- Western Boreal Initiative, Northwest Territories: <https://wbi.predictiveecology.org/apps/nwt/>
- COVID dashboard, JavaScript & data API: <https://hub.analythium.io/covidapp/>
