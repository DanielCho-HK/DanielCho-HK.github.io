---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %} -->
Below are some selected publications. You can also find my articles on <u><a href="https://scholar.google.com/citations?user=RvBDhSwAAAAJ&hl=en">my Google Scholar profile</a>.</u>
{% include base_path %}

{% for post in site.publications %}
  {% include archive-single.html %}
{% endfor %}
