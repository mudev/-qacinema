---
layout: page
title:  "New Listings"
permalink: /new-listings/
---

<ul class="post-list card-group">
	{% for p in site.data.products %}
	<li class="card">
    <h3 class="card-title">{{p.name}}</h3>
    <a href="{{p.link}}">
    <img src="{{p.image}}"/>
    </a>
    <div class="card-body">
      <span class="card-text">Actors :</span>
      <span class="card-text">{{p.actors}}</span>
    </div>
    <div class="card-body">
      <span class="card-text">Director:</span>
      <span class="card-text">{{p.director}}</span>
    </div>
    <div class="card-footer">
      <small class="text-muted">Screen Times</small>
      <small class="text-muted">{{p.screentimes}}</small>
    </div>
  </li>
	{% endfor %}	  
</ul>