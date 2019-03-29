---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find my articles on <u><a href="https://scholar.google.com/citations?user=746jY9YAAAAJ&hl=en&oi=ao">my Google Scholar profile</a>.</u>

{% include base_path %}

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
