---
layout: default
permalink: /new/
---
<div id="post_list" class="pad_size1" style="font-size: 0.8em;">
<p><h2>[NEW POST]</h2></p>	
<span>
 {% for page in site.pages %}  
	  {% if forloop.index <= 5 %}
	    <a href="https://askbrand.github.io{{ page.url }}" class="pad_size1"> - {{ page.title }}</a><br>
	  {% else %}
	  	{% break %}
	  {% endif %}
  {% endfor %}
</span>
</div>