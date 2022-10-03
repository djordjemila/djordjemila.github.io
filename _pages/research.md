---
layout: page
title: ""
permalink: /research/
---


My research interests are twofold:
* Deep learning with emphasis on probabilistic generative models, e.g. variational autoencoders.
* Applications of machine learning to real-life settings, e.g. biological and medical data.

What follows is a selection of my research projects. See also the [full & up-to-date publication list](https://scholar.google.com/citations?user=t81PmsgAAAAJ&hl=en&oi=ao).

<div>
  {% for project in site.projects reversed %}
    <hr>
    <div class="item" >
        <div class="image-fit" >
            <img class="project-img" src="{{ project.img_path | relative_url }}" alt="Ipsum Feugiat" />
        </div>
        <h5 style="text-align: left">{{project.title}}</h5>
        <header>
          <p>{% if project.paper %}<a href="{{project.paper}}">[{{project.conference}}]</a>{% endif %}
             {% if project.code %}<a href="{{project.code}}">[github]</a>{% endif %}
             {% if project.slides %}<a href="{{project.slides}}">[slides]</a>{% endif %}
             {% if project.projecter %}<a href="{{project.projecter}}">[projecter]</a>{% endif %}
             {% if project.video %}<a href="{{project.video}}">[video]</a>{% endif %}
             {% if project.workshop %}<a href="{{project.workshop_url}}">[{{project.workshop}} workshop]</a>{% endif %}
             {% if project.extra_name %}<a href="{{project.extra_url}}">[{{project.extra_name}}]</a>{% endif %}
          </p>
          <p style="font-size: 0.8em">{{project.authors}} </p>
          <p style="font-size: 0.7em;">{{project.content}}</p>
        </header>
    </div>
  {% endfor %}
</div>
