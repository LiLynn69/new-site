---
title: People
layout: collection
permalink: /people/
classes: landing
header:
  overlay_image: /assets/img/ivy.jpg
intro:
    - excerpt: 'Our interdisciplinary research team combines expertise in algorithms, networking, programming languages, systems, and verification.'
---

{% include feature_row id="intro" type="center" %}


<div class="container">
             <div class="row">
               <div class="col-sm-4 col-sm-offset-2">
                  <div class="team-member">
                    {% for person1 in site.data.people %}
                  <img src="{{ site.baseurl }} {{ person1.pic }}" class="img-responsive img-circle" alt="">
                  <h2>{{ person1.name }}</h2>
                  <h3>{{ person1.title }}</h3>
                  <p class="text-muted">{{ person1.college }}</p>
                  <ul><span class="list-inline social-buttons><li>{{ person1.links}}</li>
                  </ul>
                  {% endfor %}
                </div>
              </div>
            </div>
          <div class="row">
            <div class="col-sm-2">
                <div class="team-member">
                {% for person in site.data.people %}
                 <img src="{{ site.baseurl }} {{ person1.pic }}" class="img-responsive img-circle" alt="">
                 <h2>{{ person1.name }}</h2>
                 <h3>{{ person1.title }}</h3>
                 <p class="text-muted">{{ person1.college }}</p>
                 <ul><span class="list-inline social-buttons><li>{{ person1.links}}</li>
                 </ul>
                 {% endfor %}
              </div>
            </div>
          </div>
</div>
