---
layout: archive
title: "Working Papers"
permalink: /working-papers/
---

{% for paper in site.working-papers %}
<div style="margin-bottom: 2em;">
  <h2>
    {% if paper.paperurl %}
      <a href="{{ paper.paperurl }}" target="_blank">{{ paper.title }}</a>
    {% else %}
      <a href="{{ paper.url }}">{{ paper.title }}</a>
    {% endif %}
  </h2>
  <p><strong>{{ paper.date | date: "%Y-%m-%d" }}</strong></p>

  <div>
    {{ paper.content | markdownify }}
  </div>
</div>
<hr>
{% endfor %}
