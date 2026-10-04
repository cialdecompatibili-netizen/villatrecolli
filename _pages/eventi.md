---
layout: page
title: Eventi
nav: true
nav_order: 3
permalink: /eventi/
description: "Matrimoni, battesimi, comunioni, compleanni e meeting aziendali a Villa Tre Colli, Monterotondo."
dropdown: true
children:
  - title: "Matrimonio a Villa Tre Colli"
    permalink: /servizi/matrimonio-a-villa-tre-colli/
  - title: "divider"
    permalink: "#"
  - title: "Matrimonio civile"
    permalink: /servizi/matrimonio-civile/
  - title: "divider"
    permalink: "#"
  - title: "Battesimo, comunione e cresima"
    permalink: /servizi/battesimo-comunione-e-cresima/
  - title: "divider"
    permalink: "#"
  - title: "Compleanni e feste a tema"
    permalink: /servizi/compleanni-e-feste-a-tema/
  - title: "divider"
    permalink: "#"
  - title: "Meeting aziendali"
    permalink: /servizi/meeting-aziendali/
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

{%- assign sezione = site.servizi | where: "gruppo", "Eventi" %}
{% include servizi_tabella.liquid titolo="Eventi" lista=sezione %}
