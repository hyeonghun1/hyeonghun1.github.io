---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if author.googlescholar %} -->
<!-- {% endif %} -->

{% include base_path %}

You can also find my articles on [my Google Scholar profile](https://scholar.google.com/citations?user=sdR-LZ4AAAAJ&hl=en) and preprints on [arXiv](https://arxiv.org/search/?query=Hyeonghun+Kim&searchtype=all&abstracts=show&order=-announced_date_first&size=50).

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
