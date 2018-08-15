---
layout: page
title: Research
permalink: /research/
---

[Download my full CV (pdf)]({{ "files/hsieh-cv.pdf" | relative_url }})

# Publications
{% for pub in site.data.publications %}
- **{{ pub.year }}.**
  {% if pub.coauthor -%}
    (with {{ pub.coauthor }})
  {% endif -%}
  {{ pub.title }}.
  {% unless pub.journal -%} In {% endunless -%}
  *{{ pub.venue }}*
  {%- if pub.pages -%}, pp. {{ pub.pages }}{%- endif -%}.
  ({%- for l in pub.link -%}
    [{{ l.text }}]({{ l.url }})
    {%- if forloop.last == false %}; {% endif -%}
  {% endfor -%})
{% endfor %}


# Presentations
{% for pres in site.data.presentations %}
- **{{ pres.date | date: "%Y" }}.**
  {% if pres.coauthor -%}
    (with {{ pres.coauthor }})
  {% endif -%}
  {{ pres.title }}.
  Presented at {{ pres.venue }}, {{ pres.location }}, {{ pres.date | date: "%b %-d"}}
  {%- if pres.date_end -%}--
    {%- capture start_mo -%}{{pres.date | date: "%b " }}{%- endcapture -%}
    {%- capture end_mo -%}{{pres.date_end | date: "%b " }}{%- endcapture -%}
    {%- if start_mo != end_mo -%}
      {{ end_mo }}
    {%- endif -%}
    {{ pres.date_end | date: "%-d" }}
  {%- endif -%}.
  ({{ pres.type }}
  {%- if pres.link -%}
    ; [{{ pres.link.text }}]({{ pres.link.url | relative_url }})
  {%- endif -%})
{% endfor %}



<!-- This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](http://jekyllrb.com/)

You can find the source code for the Jekyll new theme at: [github.com/jglovier/jekyll-new](https://github.com/jglovier/jekyll-new)

You can find the source code for Jekyll at [github.com/jekyll/jekyll](https://github.com/jekyll/jekyll)
 -->
