---
title: Meditation
layout: page
permalink: /meditation
image_alt: An image of a woman meditating.
my_variable: Meditation is a great way to relax and lower stress.
---
<div class="content-left" markdown="1">
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
</div>
</div>
<div class="img-right" markdown="1">
![Image of a Woman Meditating](/assets/images/meditation.jpg)
</div>
<div class="clearfix">