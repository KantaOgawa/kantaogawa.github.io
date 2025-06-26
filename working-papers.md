---
layout: archive
title: ""
permalink: /working-papers/
---
<style>
/* === Consistent Elegant Blue Background for Working Papers Page === */
html, body {
  background-color: #edf1f5; /* 淡く上品な青みがかった背景 */
  color: #1a1a2e;
  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
}

/* Headings */
h1, h2, h3, h4, h5 {
  color: #1c2c4c;
}

/* Paper title links */
h2 a {
  color: #305c8e;
  text-decoration: none;
  border-bottom: 1px dotted #305c8e;
  transition: color 0.3s ease, border-bottom 0.3s ease;
}

h2 a:hover {
  color: #102944;
  border-bottom: 1px solid #102944;
}

/* Paper block styling */
div.paper-block {
  background-color: #ffffff;
  padding: 2rem;
  border-left: 5px solid #3a5276;
  box-shadow: 0 4px 10px rgba(26, 38, 58, 0.08);
  border-radius: 10px;
  margin-bottom: 2rem;
  box-sizing: border-box;
}

/* Horizontal line styling */
hr {
  border: none;
  border-top: 1px solid #c0c7d2;
  margin: 2rem 0;
}
</style>

{% for paper in site.working-papers %}
<div class="paper-block">
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
