---
title: Sleep
layout: page
permalink: /sleep
image_url: https://images.pexels.com/photos/57686/pexels-photo-57686.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
image_alt: An image of a bed.
my_variable: Sleep is necessary to function.
---
{% include page-image.html %}
<p> This is my page on sleep </p>
{{ page.my_variable }}

{% for resource in site.resources %}
{% if resource.category == 'sleep' %}
<h3> {{resource.title}}</h3>
<p><img src="{{resource.image}}" alt="alt text" /></p>
<p> {{resource.content}}</p>
<p>Category: {{ resource.category }}</p>
{% endif %}
 {% endfor %}