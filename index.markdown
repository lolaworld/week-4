---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Macro Polo China Tour
layout: index
---


<div id = "home">
  {% assign sorted_collections = site.collection %}
  {% for exhibit in sorted_collections %}
    <div class = "home_cell">
      <p class="desc">{{ exhibit.title }}</p>
    </div>
  {% endfor %}
</div>


 