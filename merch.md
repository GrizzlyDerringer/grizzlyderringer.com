---
title: "Merch"
nav: true
layout: "page"
---

<h3 class="section-head"><i class="fa fa-diamond" aria-hidden="true"></i> Merch</h3>


<div class="row">
  {% for item in site.data.merch %}
    <div class="col-sm-3 merch-item">
      <h5>{{ item.title }}</h5>      
      <a href="{{ item.link }}" 
         target="_blank"
         class="merch-item-thumbnail" 
         style="background-image: url({{ item.image_url  | prepend: site.basurl }})"></a>  
      <a href="{{ item.link }}" 
         class="btn btn-success btn-block">BUY NOW {{ item.price | prepend: '$' | append: '*' }}</a>
      <small>* plus shipping/handling</small>
    </div>
  {% endfor %}
</div>
  
