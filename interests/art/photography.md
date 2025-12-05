---
layout: interest
title: Photos
permalink: /interests/art/photography/
---

# 📸 Quirky Pics

A collection of fun and unusual shots I’ve taken.  
Click on any image to view in full size:

<div class="gallery">
{% assign photo_files = site.static_files | where_exp: "img", "img.path contains 'assets/images/pics/'" %}
{% assign photo_files = photo_files | sort: "name" %}
{% for img in photo_files %}
  <a href="{{ img.path }}" data-lightbox="quirky" data-title="{{ img.name | split: '.' | first }}">
    <img src="{{ img.path }}" alt="{{ img.name | split: '.' | first }}">
  </a>
{% endfor %}
</div>

<div class="back-button-wrapper">
  <a href="/interests/art" class="back-button">⬅ Back to Art</a>
</div>
