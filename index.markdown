---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title:  Macro Polo China Tour
layout: index
---


<div>
     <ul>
{% for exhibit in site.exhibits.portrait %}

<img src="{{ exhibit.image-url }}"  width = 500 height = 500> 
<p>{{ exhibit.title }} by {{ exhibit.creator }}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
<p>{{ exhibit.description }}</p>
       </ul>

</div>


   

{% for exhibit in site.exhibits.route %}
<div>
    

<img src="{{ exhibit.image-url }}"  width = 600 height = 600> 
<p>{{ exhibit.title }} by {{ exhibit.creator }}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
<p>{{ exhibit.description }}</p>

  

</div>

{% endfor %}