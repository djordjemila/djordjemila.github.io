---
title: Research Highlights
icon: fa-th
order: 2
---

<p>The first line of my research are deep generative models with the particular focus on
<a href="https://arxiv.org/abs/1906.02691">variational autoencoders</a> and deep autoregressive models.
  I explore improved techniques for learning probabilistic models (density estimation) and discovering 'useful' data representations in an unsupervised fashion. </p>

<div class="row">
  {% for post in site.posts %}
  {% if post.category=='ml' %}
     <div class="4u 12u$(mobile)">
        <div class="item" style="border: 1px solid black; height: 500px; background-color: white">
            <a href="#" class="image fit" ><img src="{{ post.img_path | relative_url }}" alt="Ipsum Feugiat" /></a>
            <header>
              <h3 style="color: black; font-size: 1em; font-family: 'Arial'">{{post.title}}</h3>
              <p style="font-size: 0.7em;">{{post.authors}} </p>
              <p style="font-size: 0.7em;">{{post.content}}</p>
              <p>{% if post.paper %}<a href="{{post.paper}}">[{{post.conference}} link]</a>{% endif %}
                 {% if post.code %}<a href="{{post.code}}">[code]</a>{% endif %}
                 {% if post.poster %}<a href="{{post.poster}}">[poster]</a>{% endif %}
                 {% if post.video %}<a href="{{post.video}}">[video]</a>{% endif %}
                 {% if post.workshop %}<a href="{{post.workshop_url}}">[{{post.workshop}} workshop]</a>{% endif %}
                 {% if post.extra_name %}<a href="{{post.extra_url}}">[{{post.extra_name}}]</a>{% endif %}
              </p>
            </header>
        </div>
     </div>
  {% endif %}
  {% endfor %}
</div>

<p>The second line of my research are the applications of deep learning to biological and medical data. I am particularly intrigued by sleep -- 
humans spend roughly one third of their lives sleeping and yet so little is known about this mysterious phenomenon. </p>

<div class="row">
  {% for post in site.posts %}
  {% if post.category=='bio' %}
     <div class="4u 12u$(mobile)">
        <div class="item" style="border: 1px solid black; height: 500px; background-color: white">
            <a href="#" class="image fit" ><img src="{{ post.img_path | relative_url }}" alt="Ipsum Feugiat" /></a>
            <header>
              <h3 style="color: black; font-size: 1em; font-family: 'Arial'">{{post.title}}</h3>
              <p style="font-size: 0.7em;">{{post.authors}} </p>
              <p style="font-size: 0.7em;">{{post.content}}</p>
              <p>{% if post.paper %}<a href="{{post.paper}}">[{{post.conference}} link]</a>{% endif %}
                 {% if post.code %}<a href="{{post.code}}">[code]</a>{% endif %}
                 {% if post.poster %}<a href="{{post.poster}}">[poster]</a>{% endif %}
                 {% if post.video %}<a href="{{post.video}}">[video]</a>{% endif %}
                 {% if post.workshop %}<a href="{{post.workshop_url}}">[{{post.workshop}} workshop]</a>{% endif %}
                 {% if post.extra_name %}<a href="{{post.extra_url}}">[{{post.extra_name}}]</a>{% endif %}
              </p>
            </header>
        </div>
     </div>
  {% endif %}
  {% endfor %}
</div>