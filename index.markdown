---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title:  Macro Polo China Tour
layout: index
---

# Macro Polo China Tour
<div>
     <ul>
{% for exhibit in site.exhibits.Macro Polo Portrait %}

<img src="{{ exhibit.image-url }}"  width = 600 height = 500> 
<p>{{ exhibit.title }} by {{ exhibit.creator }}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
<p>{{ exhibit.description }}</p>


{% for exhibit in site.exhibits.Macro Polo Portrait %}

<img src="{{ exhibit.image-url }}"  width = 600 height = 500> 
<p>{{ exhibit.title }} by {{ exhibit.creator }}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
<p>{{ exhibit.description }}</p>



{% endfor %}

