---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if author.googlescholar %} -->
  You can also find my articles on [my Google Scholar profile](https://scholar.google.com/citations?user=S_1__BUAAAAJ&hl=en&authuser=2)
  and preprints on [arXiv](https://arxiv.org/search/math?searchtype=author&query=Corbin,+N+A)
<!-- {% endif %} -->

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
