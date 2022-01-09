---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title:  Macro Polo China Tour
layout: index
---





<div id = "home">
  {% assign sorted_exhibits = site.exhibits | sort: "date" %}
  {% for exhibit in sorted_exhibits %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
    {% assign creator = site.data.creators | find: "name", exhibit.creator %}
    <div class = "item">
      <a href = "{{ exhibit.url }}"><img src="{{ exhibit.image-url }}" class="home_thumb"></a>
      <div class="info">
      <p class = "caption"><a href = "{{ exhibit.url }}">{{ exhibit.title }}</a> by <a href = "{{ creator.homepage }}">{{ exhibit.creator }}</a></p>
      <p><a href="{{ licence_url.url }}">{{ exhibit.licence }}</a></p>
      <p class="desc">{{ exhibit.description }}</p>
      </div>
    </div>
  {% endfor %}
</div>


 