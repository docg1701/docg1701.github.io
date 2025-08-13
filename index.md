---
layout: default
title: Início
---

# Bem-vindo ao meu DevLog

Este é o meu espaço para compartilhar aprendizados, projetos e ideias. Navegue pelos posts abaixo!

## Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span> - {{ post.date | date: "%d/%m/%Y" }}</span>
    </li>
  {% endfor %}
</ul>
