---
layout: default
title: Home
---

# Welcome!
I am an Assistant Professor in Linguistics at National Tsing Hua University in Taiwan.
I received my PhD from McGill University under the supervision of Junko Shimoyama, Lisa Travis, and Jessica Coon.
Prior to joining NTHU, I previously served as a postdoctoral fellow at the Hong Kong Polytechnic University and the National University of Singapore.
My main research interests lie with Tagalog, an Austronesian language spoken in the Philippines, and how it can inform our understanding of syntax and semantics.

My dissertation investigates the structure and distribution of A'-dependencies (relative clauses, _wh_-questions, etc.) in Tagalog by considering a wider ranged of data than in previous work.

My work primarily draws on elicitation and fieldwork data from native speaker (and my own) judgements, but I am always on the lookout for ways to incorporate larger amounts of data using experimental and/or computational methods.

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
