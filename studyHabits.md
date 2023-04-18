---
title: Study Habits
layout: page
permalink: /studyhabits
image_url: https://images.pexels.com/photos/159866/books-book-pages-read-literature-159866.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
image_alt: An image of a pile of books
my_variable: Forming good study habits can reduce school-related stress.
---
<div class="content-left" markdown="1">
{% include page-image.html %}
<p> This is my page on study habits </p>
{{ page.my_variable }}

{% for resource in site.resources %}
{% if resource.category == 'study habits' %}
<h3> {{resource.title}}</h3>
<p><img src="{{resource.image}}" alt="alt text" /></p>
<p> {{resource.content}}</p>
<p>Category: {{ resource.category }}</p>
{% endif %}
 {% endfor %}
</div>
<div class="clearfix">