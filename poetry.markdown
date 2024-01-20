---
layout: home
title: Poetry
permalink: /poetry/
categories: poetry
---

List of all the posts categorized as <strong>poetry</strong> on this site.

<ul>

{% for post in site.categories[page.categories] %}
  <li><a href="{{ post.url }}" target="_self" draggable="false">
  	{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    {{ post.title }} ({{ post.date | date: date_format }})
  </a></li>
{% endfor %}

</ul>