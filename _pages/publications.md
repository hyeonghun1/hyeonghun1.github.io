---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
excerpt: "Preprints"
---

<!-- {% if author.googlescholar %} -->
<!-- {% endif %} -->

{% include base_path %}

You can also find my articles on [my Google Scholar profile](https://scholar.google.com/citations?user=sdR-LZ4AAAAJ&hl=en) and preprints on [arXiv](https://arxiv.org/search/?query=Hyeonghun+Kim&searchtype=all&abstracts=show&order=-announced_date_first&size=50).

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

Preprints
======
Kim, H. and Kramer, B. (2025). Physically consistent predictive reduced-order modeling by enhancing Operator Inference with state constraints. (submitted). arXiv preprint: [arXiv:2502.03672](https://arxiv.org/abs/2502.03672).