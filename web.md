---
layout: category 
title: "Web"
category: "Web"
---
<ul class="list-group list-group-flush">
    {% for post in site.categories.web %}
      {% if post.url contains "index.html" %}
      {% else %}
    <li class="list-group-item">
            <a href="{{ post.url }}">{{ post.title }}</a>
            <span style="float:right;color:#cccccc;font-size:10px;text-align:right;">{{ post.date | date:"%Y-%m-%d" }}</span>
    </li>
      {% endif %}
    {% endfor %}
</ul>
