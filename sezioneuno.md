---
title: Sezione uno
nav_order: 2
has_children: true
nav_open: true
has_toc: false
---

# Sezione uno

Scegli una pagina dal menu a sinistra oppure da qui sotto.

## Pagine disponibili
{: .no_toc }

{% assign children = site.pages | where: "parent", page.title | sort: "nav_order" %}
<ul>
{% for child in children %}
  <li><a href="{{ child.url | relative_url }}">{{ child.title }}</a></li>
{% endfor %}
</ul>
