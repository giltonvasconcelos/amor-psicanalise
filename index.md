---
layout: default
title: "Amor e Psicanálise"
---

<!-- HEADER - HTML puro funciona em Markdown -->
<div style="position: relative; width: 100%; height: 400px; overflow: hidden; margin-bottom: 2em;">
    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='1200' height='400' viewBox='0 0 1200 400'%3E%3Cdefs%3E%3ClinearGradient id='g' x1='0%25' y1='0%25' x2='100%25' y2='100%25'%3E%3Cstop offset='0%25' stop-color='%236b8c9f'/%3E%3Cstop offset='100%25' stop-color='%23a8c6b0'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='1200' height='400' fill='url(%23g)'/%3E%3C/svg%3E" 
         alt="Header Background" style="width: 100%; height: 100%; object-fit: cover;">
    <div style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; background: rgba(58, 42, 34, 0.6); color: white; padding: 1em;">
        <h1 style="font-size: 3em; margin: 0; text-shadow: 2px 2px 4px rgba(0,0,0,0.5);">Amor e Psicanálise</h1>
        <p style="font-size: 1.3em; margin: 1em 0 0; text-shadow: 1px 1px 2px rgba(0,0,0,0.5);">Um espaço para o encontro entre o sentir e o pensar</p>
    </div>
</div>

<!-- CARDS - Espaço entre header e cards -->
<div style="max-width: 1200px; margin: 3em auto; padding: 0 1em;">

<!-- LINHA 1 DE CARDS -->
<div style="display: flex; flex-wrap: wrap; gap: 1.5em; justify-content: center; margin-bottom: 1.5em;">
    <!-- Card 1 -->
    <a href="/amor-psicanalise/a-psicanalise/" style="flex: 1 1 200px; background: #faf7f2; border-radius: 8px; padding: 1.5em; text-decoration: none; color: #3a2a22; border: 1px solid #e5d9d0; transition: transform 0.3s; display: block; text-align: center;">
        <span style="font-size: 2.5em; display: block; margin-bottom: 0.5em;">🎯</span>
        <h3 style="margin: 0.5em 0; color: #5a4a42;">A Psicanálise</h3>
        <p style="margin: 0; color: #666;">Fundamentos e propósitos da prática psicanalítica</p>
    </a>
    
    <!-- Card 2 -->
    <a href="/amor-psicanalise/artigos/" style="flex: 1 1 200px; background: #faf7f2; border-radius: 8px; padding: 1.5em; text-decoration: none; color: #3a2a22; border: 1px solid #e5d9d0; transition: transform 0.3s; display: block; text-align: center;">
        <span style="font-size: 2.5em; display: block; margin-bottom: 0.5em;">📝</span>
        <h3 style="margin: 0.5em 0; color: #5a4a42;">Artigos & Reflexões</h3>
        <p style="margin: 0; color: #666;">Textos sobre psicanálise, amor e autoconhecimento</p>
    </a>
    
    <!-- Card 3 -->
    <a href="/amor-psicanalise/sobre/" style="flex: 1 1 200px; background: #faf7f2; border-radius: 8px; padding: 1.5em; text-decoration: none; color: #3a2a22; border: 1px solid #e5d9d0; transition: transform 0.3s; display: block; text-align: center;">
        <span style="font-size: 2.5em; display: block; margin-bottom: 0.5em;">📖</span>
        <h3 style="margin: 0.5em 0; color: #5a4a42;">Sobre esse Projeto</h3>
        <p style="margin: 0; color: #666;">História e inspiração por trás deste espaço</p>
    </a>
</div>

<!-- LINHA 2 DE CARDS -->
<div style="display: flex; flex-wrap: wrap; gap: 1.5em; justify-content: center;">
    <!-- Card 4 -->
    <a href="/amor-psicanalise/faq/" style="flex: 1 1 200px; background: #faf7f2; border-radius: 8px; padding: 1.5em; text-decoration: none; color: #3a2a22; border: 1px solid #e5d9d0; transition: transform 0.3s; display: block; text-align: center;">
        <span style="font-size: 2.5em; display: block; margin-bottom: 0.5em;">❓</span>
        <h3 style="margin: 0.5em 0; color: #5a4a42;">Perguntas Frequentes</h3>
        <p style="margin: 0; color: #666;">Respostas para as principais dúvidas</p>
    </a>
    
    <!-- Card 5 -->
    <a href="/amor-psicanalise/contato/" style="flex: 1 1 200px; background: #faf7f2; border-radius: 8px; padding: 1.5em; text-decoration: none; color: #3a2a22; border: 1px solid #e5d9d0; transition: transform 0.3s; display: block; text-align: center;">
        <span style="font-size: 2.5em; display: block; margin-bottom: 0.5em;">📧</span>
        <h3 style="margin: 0.5em 0; color: #5a4a42;">Contato</h3>
        <p style="margin: 0; color: #666;">Entre em contato comigo</p>
    </a>
</div>

</div>

<!-- POSTS RECENTES -->
<div style="max-width: 800px; margin: 4em auto; padding: 0 1em;">
    <h2 style="text-align: center; color: #3a2a22; font-size: 2em; margin-bottom: 1.5em;">📝 Reflexões Recentes</h2>
    
    {% for post in site.posts limit:3 %}
    <div style="background: #faf7f2; border-left: 4px solid #d4a5a5; padding: 1.5em; margin-bottom: 1.5em; border-radius: 0 8px 8px 0;">
        <h3 style="margin-top: 0; margin-bottom: 0.5em;"><a href="{{ post.url }}" style="color: #3a2a22; text-decoration: none;">{{ post.title }}</a></h3>
        <div style="color: #999; font-size: 0.85em; margin-bottom: 1em;">{{ post.date | date: "%d/%m/%Y" }}</div>
        <div style="color: #666; line-height: 1.6;">
            {{ post.excerpt | strip_html | truncate: 150 }}
        </div>
    </div>
    {% endfor %}
    
    <div style="text-align: center; margin-top: 2em;">
        <a href="/amor-psicanalise/artigos/" style="background: #d4a5a5; color: white; padding: 0.8em 2em; text-decoration: none; border-radius: 4px; display: inline-block;">Ver todos os artigos</a>
    </div>
</div>

<!-- FOOTER -->
<div style="background: #3a2a22; color: #f5f0e8; padding: 2em 1em; margin-top: 3em; text-align: center;">
    <div style="margin-bottom: 1em;">
        <a href="/amor-psicanalise/termos-de-uso/" style="color: #d4a5a5; text-decoration: none; margin: 0 1em;">Termos de Uso</a>
        <a href="/amor-psicanalise/politica-de-privacidade/" style="color: #d4a5a5; text-decoration: none; margin: 0 1em;">Política de Privacidade</a>
    </div>
    <div style="font-size: 0.85em; color: #a89b92;">
        © 2026 Gilton Vasconcelos. Todos os direitos reservados.
    </div>
</div>
