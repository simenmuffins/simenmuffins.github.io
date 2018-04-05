---
layout: default
---
# Portfolio

<div class="row gallery">
  {% assign image_files = site.static_files | where: "image", true %}
  {% for myimage in image_files %}
  <div class="col-6">
    <a href="{{ myimage.path }}" data-lightbox="portfolio">
      <img src="{{ myimage.path }}" class="img-fluid" />
    </a>
  </div>
  {% endfor %}
</div>
