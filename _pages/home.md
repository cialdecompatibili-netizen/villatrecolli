---
layout: about
title: Home
permalink: /
nav: true
nav_order: 0.3

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false

announcements:
  enabled: false
  scrollable: true
  limit: 5

latest_posts:
  enabled: true
  scrollable: true
  limit: 3
seo_title: "{title} | Location per matrimoni ed eventi a Monterotondo, Roma"
seo_description: "Villa Tre Colli è una location Ideale per feste ed eventi privati situata a due passi da Roma, nella ridente cittadina di Monterotondo <3"
---

<style>
.post-header{display:none}
.vh-hero{text-align:center;padding:3rem 0 1.5rem}
.vh-hero h2{margin-top:0}
.vh-hero p{max-width:720px;margin:0 auto 1rem}
.vh-btns{display:flex;flex-wrap:wrap;gap:12px;justify-content:center;margin-top:1.6rem}
.vh-btns a{display:inline-block;padding:.6rem 1.5rem;border-radius:999px;border:1px solid rgba(0,0,0,.25);text-decoration:none;font-weight:600}
.vh-btns a.vh-main{background:#2f5d50;border-color:#2f5d50;color:#fff}
html[data-theme="dark"] .vh-btns a{border-color:rgba(255,255,255,.35)}
.vh-num{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;max-width:900px;margin:1.5rem auto 0;text-align:center}
.vh-num div{padding:14px 10px;border:1px solid rgba(0,0,0,.12);border-radius:12px;background:#fffdf5}
.vh-num b{display:block;font-size:1.15rem}
.vh-num small{opacity:.7}
html[data-theme="dark"] .vh-num div{background:rgba(255,255,255,.05);border-color:rgba(255,255,255,.15)}
.vh-info{max-width:900px;margin:2.5rem auto;text-align:center}
@media (max-width:700px){.vh-num{grid-template-columns:1fr 1fr}}

.srv-home{margin:2.5rem 0}
.srv-home h2{text-align:center;margin-bottom:1.4rem}
.srv-home-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;max-width:900px;margin:0 auto}
.srv-home-card{display:block;color:inherit;text-decoration:none;padding:16px 18px;border:1px solid rgba(0,0,0,.12);border-radius:12px;background:#fffdf5;text-align:left}
.srv-home-card b{display:block;margin-bottom:4px}
.srv-home-card small{opacity:.65;display:block}
html[data-theme="dark"] .srv-home-card{background:rgba(255,255,255,.05);border-color:rgba(255,255,255,.15)}
.srv-home-more{text-align:center;margin-top:1.6rem}
.srv-home-more a{display:inline-block;padding:.55rem 1.4rem;border-radius:999px;border:1px solid rgba(0,0,0,.2);text-decoration:none;font-weight:600}
html[data-theme="dark"] .srv-home-more a{border-color:rgba(255,255,255,.3)}
@media (max-width:700px){.srv-home-grid{grid-template-columns:1fr}}
</style>

<div class="vh-hero" markdown="1">

## Benvenuti a Villa Tre Colli

Alle porte di Roma, nella prosperosa e ridente cittadina di Monterotondo, considerata da molti una tra le maggiori realtà storiche dal grande rilievo artistico e culturale, nei pressi della capitale, sorge immersa in un eden di serenità e natura, circondata da uno splendido paesaggio collinare, Villa Tre Colli.

[Leggi tutto]({{ '/servizi/la-villa/' | relative_url }})

<div class="vh-btns">
<a class="vh-main" href="{{ '/contatti/' | relative_url }}">Richiedi un preventivo</a>
<a href="tel:+393338495178">Chiama 333 849 5178</a>
<a href="{{ '/servizi/' | relative_url }}">Scopri la villa</a>
</div>

<div class="vh-num">
<div><b>Fino a 250</b><small>ospiti nella Sala Grande</small></div>
<div><b>2 sale</b><small>collegate tra loro</small></div>
<div><b>Cucina interna</b><small>piatti preparati sul posto</small></div>
<div><b>Uso esclusivo</b><small>la villa è solo per il tuo evento</small></div>
</div>

</div>

{%- assign srv_home = site.servizi | where: 'in_home', 'true' | sort: 'ordine' -%}
{%- if srv_home.size > 0 %}
<div class="srv-home">
  <h2>Per ogni occasione</h2>
  <div class="srv-home-grid">
    {%- for p in srv_home -%}
    <a class="srv-home-card" href="{{ p.url | relative_url }}"><b>{{ p.title | escape }}</b>{% if p.sottotitolo != blank %}<small>{{ p.sottotitolo | escape }}</small>{% elsif p.description != blank %}<small>{{ p.description | truncatewords: 8 | escape }}</small>{% endif %}</a>
    {%- endfor %}
  </div>
  <div class="srv-home-more">
    <a href="{{ '/servizi/' | relative_url }}">Vedi tutta la villa e i servizi</a>
  </div>
</div>
{%- endif %}

<div class="vh-info" markdown="1">

## Dove siamo

**Villa Tre Colli**, Via Guerrazzi 103, 00015 Monterotondo (Roma).
Telefono: [333 849 5178](tel:+393338495178), email: [info@villatrecolli.com](mailto:info@villatrecolli.com).

[Come raggiungerci]({{ '/contatti/' | relative_url }})

</div>
