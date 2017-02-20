---
title: "Merch"
nav: true
layout: "page"
---

<h3 class="section-head"><i class="fa fa-diamond" aria-hidden="true"></i> Merch</h3>


<div class="row">
  {% for item in site.data.merch %}
    <div class="col-sm-3">
      {{ item.img_url }}
      <a href="{{ item.link }}">    
        <img src="{{ item.image_url | prepend: site.basurl }}" alt="{{ item.title }}" class="img-responsive">
      </a>  
    </div>
  {% endfor %}
</div>
  
