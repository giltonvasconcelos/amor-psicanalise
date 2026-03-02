---
layout: archive
title: "Artigos e Reflexões"
permalink: /artigos/
author_profile: true
---

Este espaço reúne palavras que tocam, questionam e inspiram.

Cada texto é um convite para desacelerar, respirar e enxergar a vida por ângulos
diferentes. Aqui, reflexões se transformam em janelas abertas para o sentir e o pensar.

---

{% assign posts = site.posts %}
{% if posts.size > 0 %}
  {% for post in posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p><small>{{ post.date | date: "%d/%m/%Y" }}</small></p>
    <p>{{ post.excerpt }}</p>
  </article>
  <hr>
  {% endfor %}
{% else %}
  <p>Em breve, novos artigos e reflexões serão publicados aqui. Volte logo! 💙</p>
{% endif %}
