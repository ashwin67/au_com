---
layout: full-width
title: Old
# Note that this index page uses a full-width layout!
---

  <h1 class="content-listing-header sans">Archived Posts</h1>
  <ul class="content-listing ">
    {% for post in site.posts %}    
	  {% if post.categories %}
	    {% assign archived = 0 %}
	    {% for category in post.categories %}
	      {% if category == "Archived" %}
		{% assign archived = 1 %}
	      {% endif %}
	    {% endfor %}
	    {% if archived == 1 %}  
		<li class="listing">
		  <hr class="slender">
		  <a href="{{ post.url | prepend: site.baseurl }}"><h3 class="contrast">{{ post.title }}</h3></a>
		  <br><span class="smaller">{{ post.date | date: "%B %-d, %Y" }}</span>  <br/>
		  <div>{{ post.excerpt }}</div> 
		</li>
            {% endif %}
          {% endif %}
        {% endfor %}
  </ul>
