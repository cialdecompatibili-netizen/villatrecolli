---
layout: page
title: La villa
nav: true
nav_order: 1
permalink: /la-villa/
description: "La villa, le sale, la cucina interna, lo spazio esterno e il Tunnel dell’Amore di Villa Tre Colli a Monterotondo."
seo_title: "La villa e i suoi spazi: sale, cucina e giardino | Villa Tre Colli"
dropdown: true
children:
  - title: "La villa"
    permalink: /servizi/la-villa/
  - title: "divider"
    permalink: "#"
  - title: "Le sale di Villa Tre Colli"
    permalink: /servizi/le-sale-di-villa-tre-colli/
  - title: "divider"
    permalink: "#"
  - title: "La cucina interna"
    permalink: /servizi/la-cucina-interna/
  - title: "divider"
    permalink: "#"
  - title: "Lo spazio esterno"
    permalink: /servizi/lo-spazio-esterno/
  - title: "divider"
    permalink: "#"
  - title: "Il Tunnel dell’Amore"
    permalink: /servizi/il-tunnel-dellamore/
---

<style>
.srv-t{width:100%;border-collapse:separate;border-spacing:8px;margin:6px 0 26px}
.srv-t td{width:33.33%;padding:9px 12px;border:1px solid rgba(0,0,0,.12);border-radius:10px;background:#fffdf5;font-size:.9rem;line-height:1.3;vertical-align:top}
.srv-t td small{display:block;opacity:.65}
.srv-t td:empty{background:none;border:0}
.srv-t td{position:relative}
.srv-t td a{color:inherit;text-decoration:none}
.srv-t td a::after{content:"";position:absolute;top:0;right:0;bottom:0;left:0;border-radius:10px}
html[data-theme="dark"] .srv-t td{background:rgba(255,255,255,.05);border-color:rgba(255,255,255,.15)}
@media(max-width:600px){.srv-t,.srv-t tbody,.srv-t tr,.srv-t td{display:block;width:100%}.srv-t{border-spacing:0}.srv-t td{margin-bottom:6px}.srv-t td:empty{display:none}}
</style>

{%- assign sezione = site.servizi | where: "gruppo", "La villa" %}
{% include servizi_tabella.liquid titolo="La villa" lista=sezione %}
