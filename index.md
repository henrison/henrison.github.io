---
layout: default
title: Home
---

# Welcome!

My name is Thanh Viet Cao (Vietnamese: Cao Thành Việt). I am a seventh-year PhD candidate at the Graduate Institute of Linguistics, National Tsing Hua University, Taiwan, under the supervision of Prof. I-Ta Chris Hsieh. Before that, I got both a B.A. and an M.A. in linguistics from the Faculty of Linguistics, University of Social Sciences and Humanities, Vietnam National University (VNU, Hanoi). My main research interests include semantics, pragmatics, and syntax of classifier languages in light of formal approaches, i.e., model-theoretical semantics and comparative syntax within the framework of generative grammar. At the moment, I am preparing for my PhD dissertation oral defense (title: **Quantification and Plurality at the Interface: The case of Vietnamese**), which will be held on May 14th, 2025. My thesis mainly touches upon strategies of universal quantification (involving the four D-quantifiers *tất-cả*, *cả*, *mọi*, and *mỗi*) and plurality (involving *các* and *những*) in Vietnamese from compositional and cross-linguistic perspectives. Besides, language contact among MSEA languages from historical linguistics aspects, especially the historical lexicology (i.e., etymology) of the Vietnamese lexicon, always attracts my attention from time to time.

<!-- Last updated: {{ site.last_updated | date: "%b %Y" }} -->

## Recent and upcoming

{% for entry in site.data.updates limit:4 %}
  - **{{ entry.date | date: "%b %Y" }}:** {{ entry.text -}}
{%- endfor %}



{% comment %}
>>> Keeping this for posterity in case I want to set up some kind of post repository
<h1 class="page-heading">Posts</h1>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
{% endcomment %}
