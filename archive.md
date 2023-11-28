---
layout: page
title: About
---
The Machine Learning for Data-driven Optimization workshop focuses on the emerging field of machine learning for data-driven optimization. We aim to bring together researchers from various disciplines to explore novel theories, algorithms, and applications in data-driven optimization. As optimization plays an increasingly important role in science and engineering, this workshop will provide a platform for experts from both academia and industry to discuss promises and challenges in solving complex optimization problems using machine learning techniques and data-driven optimization.

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
