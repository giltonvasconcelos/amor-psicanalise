---
layout: default
title: "Amor e Psicanálise"
---

<div class="header">
    <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='1200' height='400' viewBox='0 0 1200 400'%3E%3Cdefs%3E%3ClinearGradient id='g' x1='0%25' y1='0%25' x2='100%25' y2='100%25'%3E%3Cstop offset='0%25' stop-color='%236b8c9f'/%3E%3Cstop offset='100%25' stop-color='%23a8c6b0'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='1200' height='400' fill='url(%23g)'/%3E%3C/svg%3E" 
         alt="Header Background" class="header-image">
    <div class="header-overlay">
        <h1>Amor e Psicanálise</h1>
        <p>Um espaço para o encontro entre o sentir e o pensar</p>
    </div>
</div>

<div class="menu-cards">
    <a href="/amor-psicanalise/a-psicanalise/" class="menu-card">
        <span class="emoji">🎯</span>
        <h3>A Psicanálise</h3>
        <p>Fundamentos e propósitos da prática psicanalítica</p>
    </a>
    <a href="/amor-psicanalise/artigos/" class="menu-card">
        <span class="emoji">📝</span>
        <h3>Artigos & Reflexões</h3>
        <p>Textos sobre psicanálise, amor e autoconhecimento</p>
    </a>
    <a href="/amor-psicanalise/sobre/" class="menu-card">
        <span class="emoji">📖</span>
        <h3>Sobre esse Projeto</h3>
        <p>História e inspiração por trás deste espaço</p>
    </a>
    <a href="/amor-psicanalise/faq/" class="menu-card">
        <span class="emoji">❓</span>
        <h3>Perguntas Frequentes</h3>
        <p>Respostas para as principais dúvidas</p>
    </a>
    <a href="/amor-psicanalise/contato/" class="menu-card">
        <span class="emoji">📧</span>
        <h3>Contato</h3>
        <p>Entre em contato comigo</p>
    </a>
</div>

<div class="recent-posts">
    <h2>📝 Reflexões Recentes</h2>
    
    {% for post in site.posts limit:3 %}
    <div class="post-item">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <div class="post-meta">{{ post.date | date: "%d/%m/%Y" }}</div>
        <div class="post-excerpt">
            {{ post.excerpt | strip_html | truncate: 150 }}
        </div>
    </div>
    {% endfor %}
    
    <div style="text-align: center; margin-top: 2em;">
        <a href="/amor-psicanalise/artigos/" class="btn">Ver todos os artigos</a>
    </div>
</div>

<footer class="footer">
    <div class="footer-links">
        <a href="/amor-psicanalise/termos-de-uso/">Termos de Uso</a>
        <a href="/amor-psicanalise/politica-de-privacidade/">Política de Privacidade</a>
    </div>
    <div class="copyright">
        © 2026 Gilton Vasconcelos. Todos os direitos reservados.
    </div>
</footer>

<style>
.header {
    position: relative;
    width: 100%;
    height: 400px;
    overflow: hidden;
    margin-bottom: 2em;
}
.header-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.header-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: rgba(58, 42, 34, 0.6);
    color: white;
    padding: 1em;
}
.header-overlay h1 {
    font-size: 3em;
    margin: 0;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
}
.header-overlay p {
    font-size: 1.3em;
    margin: 1em 0 0;
    text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
}
.menu-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5em;
    max-width: 1200px;
    margin: 3em auto;
    padding: 0 1em;
}
.menu-card {
    background: #faf7f2;
    border-radius: 8px;
    padding: 1.5em;
    text-decoration: none;
    color: #3a2a22;
    transition: transform 0.3s, box-shadow 0.3s;
    border: 1px solid #e5d9d0;
    display: block;
}
.menu-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    background: #f5f0e8;
}
.menu-card .emoji {
    font-size: 2.5em;
    display: block;
    margin-bottom: 0.5em;
}
.menu-card h3 {
    margin: 0.5em 0;
    color: #5a4a42;
    font-size: 1.3em;
}
.menu-card p {
    margin: 0;
    color: #666;
    font-size: 0.9em;
    line-height: 1.5;
}
.recent-posts {
    max-width: 800px;
    margin: 4em auto;
    padding: 0 1em;
}
.recent-posts h2 {
    text-align: center;
    color: #3a2a22;
    font-size: 2em;
    margin-bottom: 1.5em;
}
.post-item {
    background: #faf7f2;
    border-left: 4px solid #d4a5a5;
    padding: 1.5em;
    margin-bottom: 1.5em;
    border-radius: 0 8px 8px 0;
}
.post-item h3 {
    margin-top: 0;
    margin-bottom: 0.5em;
}
.post-item h3 a {
    color: #3a2a22;
    text-decoration: none;
    font-size: 1.2em;
}
.post-item h3 a:hover {
    color: #d4a5a5;
}
.post-meta {
    color: #999;
    font-size: 0.85em;
    margin-bottom: 1em;
}
.post-excerpt {
    color: #666;
    line-height: 1.6;
    margin: 0.5em 0;
}
.footer {
    background: #3a2a22;
    color: #f5f0e8;
    padding: 2em 1em;
    margin-top: 3em;
    text-align: center;
}
.footer-links {
    margin-bottom: 1em;
}
.footer-links a {
    color: #d4a5a5;
    text-decoration: none;
    margin: 0 1em;
    font-size: 0.9em;
}
.footer-links a:hover {
    text-decoration: underline;
}
.copyright {
    font-size: 0.85em;
    color: #a89b92;
}
.btn {
    background: #d4a5a5;
    color: white;
    padding: 0.8em 2em;
    text-decoration: none;
    border-radius: 4px;
    display: inline-block;
    transition: background 0.3s;
}
.btn:hover {
    background: #b58b8b;
}
@media (max-width: 768px) {
    .header-overlay h1 {
        font-size: 2em;
    }
    .header-overlay p {
        font-size: 1em;
    }
    .menu-cards {
        grid-template-columns: 1fr;
    }
    .footer-links a {
        display: block;
        margin: 0.5em 0;
    }
}
</style>
