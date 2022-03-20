---
layout: archive
title: "Students"
permalink: /students/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}
## Ph.D Students
{% assign stus = site.students | where: 'role', 'Phd' %}
{% for stu in stus %}
{{ stu }}
{% endfor %}

## Master Students
{% assign stus = site.students | where: 'role', 'Master' %}
{% for stu in stus %}
{{ stu }}
{% endfor %}

## Undergraduate Students
{% assign stus = site.students | where: 'role', 'Undergraduate' %}
{% for stu in stus %}
{{ stu }}
{% endfor %}

## Alumni
{% assign stus = site.students | where: 'role', 'Graduated' %}
{% for stu in stus %}
{{ stu }}
{% endfor %}