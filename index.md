---
layout: default
title: "Amor e Psicanálise"
---

# Amor e Psicanálise

*Entre o inconsciente e o amor, novos caminhos de autenticidade*

---

## Menu

- [🎯 A Psicanálise](/amor-psicanalise/a-psicanalise/)
- [📝 Artigos e Reflexões](/amor-psicanalise/artigos/)
- [📖 Sobre esse Projeto](/amor-psicanalise/sobre/)
- [❓ Perguntas Frequentes](/amor-psicanalise/faq/)
- [📧 Contato](/amor-psicanalise/contato/)

---

## Reflexões Recentes

{% for post in site.posts limit:3 %}
### [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%d/%m/%Y" }}*

{{ post.excerpt | strip_html | truncate: 150 }}

[Leia mais →]({{ post.url }})

---
{% endfor %}

[Ver todos os artigos](/amor-psicanalise/artigos/)

---

<div style="text-align: center; font-size: 0.9em; color: #666;">
    © 2026 Gilton Vasconcelos<br>
    <a href="/amor-psicanalise/termos-de-uso/">Termos de Uso</a> | 
    <a href="/amor-psicanalise/politica-de-privacidade/">Política de Privacidade</a>
</div>
