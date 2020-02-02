---
title: People
layout: collection
permalink: /people/
classes: landing
header:
  overlay_image: /assets/images/ruth-bike.jpg
intro:
    - excerpt: 'Our interdisciplinary research team combines expertise in algorithms, networking, programming languages, systems, and verification.'
---

{% include feature_row id="intro" type="center" %}

{% assign person1 = site.data.people | where:'type','person1' %}
{% assign person = site.data.people | where:'type','person' %}



<div class="container">
             <div class="row">
               <div class="col-sm-4 col-sm-offset-2">
                  <div class="team-member">
                      <ul>        
                        {% for bio in person1 %}
                        {% include people.html %}
                        {% endfor %}
                     </ul>
                </div>
              </div>
            </div>
          <div class="row">
            <div class="col-sm-2">
                <div class="team-member">
                  <ul>        
                    {% for bio in person %}
                    {% include people.html %}
                    {% endfor %}
                 </ul>
              </div>
            </div>
          </div>
</div>
