---
collection: menu
title: Research
permalink: /research/
---

# Research

You can find a list of my publications and presentations below with relevant links to the paper or handout/slides, where available.
Please feel free to email me if there is something you're looking for that is not listed below!

## Dissertation
  **2020.**
  Beyond Nominative: A broader view of Tagalog A'-dependencies.
  McGill University.\\
  ([pdf](/files/thesis-pdfx.pdf),
    [lingbuzz](https://lingbuzz.net/lingbuzz/005856),
    [eScholarship@McGill](https://escholarship.mcgill.ca/concern/theses/2z10ww16v))


## Publications
{% for pub in site.data.publications %}
- **{{ pub.year }}.**
  {% if pub.coauthor -%}
    (with {{ pub.coauthor }})
  {% endif -%}
  {{ pub.title }}.
  {% unless pub.journal -%} In {% endunless -%}
  *{{ pub.venue }}*{% if pub.volume %} {{ pub.volume }}{% endif -%}
  {%- if pub.pages -%}, pp. {{ pub.pages }}{%- endif -%}.
  {% if pub.link %}({%- for l in pub.link -%}
    [{{ l.text }}]({{ l.url }})
    {%- if forloop.last == false %}; {% endif -%}
  {% endfor -%}){% endif -%}
{% endfor %}


## Presentations
{% for pres in site.data.presentations %}
- **{{ pres.date | date: "%Y" }}.**
  {{ pres.title }}.<br />
  {%- if pres.coauthor -%}
    with {{ pres.coauthor }};
  {% endif -%}
  @ _{{ pres.venue }}_, {{ pres.location }}.{%- comment -%}
  {%- endcomment %}
  ({{ pres.type }}
  {%- if pres.link -%}
    ; [{{ pres.link.text }}]({{ pres.link.url | relative_url }})
  {%- endif -%})
{%- endfor %}



<!-- This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](http://jekyllrb.com/)

You can find the source code for the Jekyll new theme at: [github.com/jglovier/jekyll-new](https://github.com/jglovier/jekyll-new)

You can find the source code for Jekyll at [github.com/jekyll/jekyll](https://github.com/jekyll/jekyll)
 -->
