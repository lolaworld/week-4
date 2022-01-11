---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Macro Polo China Tour
layout: index
---


<div id = "macro">
   {% assign sorted_exhibits = site.exhibit %} 
   {% for exhibit in sorted_exhibits %}
    <div class="item">
    <div class="title">{{ exhibit.title }}</div>
      <div class="image"><img src="{{ exhibit.image-url}}"/></div>
      <div class="info">
        <div class="creator">
          <span class="author">{{ exhibit.creator }}</span><a class="licence" href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a>
        </div>
        <div class="desc">{{ exhibit.description }}</div>
      </div>
    </div>
{% endfor %}
</div>


<div class="home-books">
<h2>Different versions of Marco Polo's travels</h2>
{% assign books = site.collection | where:"page-location","home" %}
{% for book in books %}
  <div class="item">
    <div class="title"> <a href="{{ book.url }}">{{ book.title }}</a></div>
    <div class="author">{{ book.auhtor }}</div>
  </div>
{% endfor %}
</div>
 