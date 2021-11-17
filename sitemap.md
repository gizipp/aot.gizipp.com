---
layout: page
title: Sitemap
permalink: /sitemap/
---

<amp-img width="600" height="300" layout="responsive" src="/assets/posts/ibu-dan-bayi.jpg" alt="Tentang Ibu dan Anak "></amp-img>

Sitemap atau Peta Situs Bukan tempat baca manga attack on titan dan nonton online gratis. Hanya seru-seruan saja. :)

### Artikel

<br>
<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

### Halaman

{% assign sitemap_pages = site.pages | where: "sitemap", "true" %}

<br>
<ul>
  {% for page in sitemap_pages  %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endfor %}
</ul>
