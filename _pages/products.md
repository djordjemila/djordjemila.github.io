---
layout: page
title: ""
permalink: /products/
---

<div style="font-style: italic; font-size: 0.9em;">
“Science is but a perversion of itself unless it has as its ultimate goal the betterment of humanity.”
<br>
<br>
- Nikola Tesla
</div>
<br>
The ultimate goal of my work is to create "intelligent" software that automates processes in business or science while at the same time achieving (at least) human-like performance. 
Here are a couple of examples:

<div>
  {% for product in site.products reversed %}
    <hr>
    <div class="item" >
        <div class="image-fit" >
            <img class="product-img" src="{{ product.img_path | relative_url }}" alt="Ipsum Feugiat" />
        </div>
        <h5 style="text-align: left"><a href="{{product.webpage}}">{{product.title}}</a>{% if product.url %}{% endif %}</h5>
        <p style="font-size: 0.7em;">{{product.content}}</p>
    </div>
  {% endfor %}
</div>
