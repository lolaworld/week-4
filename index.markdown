---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title:  Macro Polo China Tour
layout: index
---

{% for exhibit in site.Macro Polo Portrait %}

<img src="{{ exhibit.image-url }}"  width = 256> 
<p>{{ exhiibit.title }} by {{ exhibit.creator }}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
Macro Polo (1254~1324)

{% for exhibit in site.Macro Polo Route %}

<img src="{{ exhibit.image-url }}"  width = 500> 
<p>{{ exhiibit.title }} by {{ exhibit.creator }}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
Route of Macro Polo

{% endfor %}

