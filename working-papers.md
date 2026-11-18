---
layout: archive
title: "Working Papers"
academic_style: true
author_profile: false
permalink: /working-papers/
---
{% for paper in site.working-papers %}
<article class="paper-block">
  <h2>
    {% if paper.paperurl %}
      <a href="{{ paper.paperurl }}" target="_blank">{{ paper.title }}</a>
    {% else %}
      <a href="{{ paper.url }}">{{ paper.title }}</a>
    {% endif %}
  </h2>
  <time class="paper-date" datetime="{{ paper.date | date: "%Y-%m-%d" }}">{{ paper.date | date: "%B %-d, %Y" }}</time>

  <div>
    {{ paper.content | markdownify }}
  </div>
</article>
{% endfor %}
