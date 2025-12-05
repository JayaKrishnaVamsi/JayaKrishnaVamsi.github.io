---
layout: default
title: My Drawings
description: A collection of my drawings rendered dynamically.
permalink: /interests/art/drawings/
---

# 🎨 My Drawings
Click on any image to view in full size:

<div class="gallery">
  {% assign drawings = site.static_files | where_exp: "file", "file.path contains '/assets/images/drawings/'" %}
  {% for image in drawings %}
    <a href="{{ image.path }}" data-lightbox="drawings" data-title="{{ image.name | split: '.' | first | capitalize }}">
      <img src="{{ image.path }}" alt="{{ image.name | split: '.' | first | capitalize }}">
    </a>
  {% endfor %}
</div>

<style>
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 15px;
  justify-items: center;
  align-items: center;
  margin-top: 20px;
}

.gallery img {
  width: 250px;
  height: 250px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.gallery img:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 14px rgba(0, 0, 0, 0.3);
}
</style>


<div class="back-button-wrapper">
  <a href="/interests/art" class="back-button">⬅ Back to Art</a>
</div>
