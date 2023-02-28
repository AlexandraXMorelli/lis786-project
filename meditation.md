---
title: Meditation
layout: page
permalink: /meditation
image_url: https://images.pexels.com/photos/2908175/pexels-photo-2908175.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
image_alt: An image of a woman meditating.
my_variable: Meditation is a great way to relax and lower stress.
---
{% include page-image.html %}
<p> This is my page on meditation. </p>
{{ page.my_variable }}

{% for resource in site.resources %}
{% if resource.category == 'meditation' %}
<h3> {{resource.title}}</h3>
<p><img src="{{resource.image}}" alt="alt text" /></p>
<p> {{resource.content}}</p>
<p>Category: {{ resource.category }}</p>
{% endif %}
 {% endfor %}