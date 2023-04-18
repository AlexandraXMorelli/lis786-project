---
title: Scheduling
layout: page
permalink: /scheduling
image_url: https://images.pexels.com/photos/273153/pexels-photo-273153.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
image_alt: An image of a planner.
my_variable: Sticking to a schedule can help you manage your time better.
---
<div class="content-left" markdown="1">
{% include page-image.html %}
<p> This is my page on scheduling </p>
{{ page.my_variable }}

{% for resource in site.resources %}
{% if resource.category == 'scheduling' %}
<h3> {{resource.title}}</h3>
<p><img src="{{resource.image}}" alt="alt text" /></p>
<p> {{resource.content}}</p>
<p>Category: {{ resource.category }}</p>
{% endif %}
 {% endfor %}
</div>
<div class="clearfix">