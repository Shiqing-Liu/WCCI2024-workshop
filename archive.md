---
layout: page
title: About
---
IEEE WCCI 2024 is the world’s largest technical event on computational intelligence, featuring the three flagship conferences of the IEEE Computational Intelligence Society (CIS) under one roof: The International Joint Conference on Neural Networks (IJCNN), the IEEE International Conference on Fuzzy Systems (FUZZ-IEEE) and the IEEE Congress on Evolutionary Computation (IEEE CEC).

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
