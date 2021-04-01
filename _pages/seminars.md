---
layout: page
title: seminars
permalink: /seminars/
description: Veronesi Tutti Math (VTM) series
nav: true
---

The first meeting that should have happened in May 2020 was canceled because of the well known situation. Since we can not predict when we will have our first in-person meeting, we'd better start off with some online occasion to see each other and talk about things that we are all passionate about.
Together with the [Collegio Didattico di Matematica](https://www.di.univr.it/?ent=organo&id=657) of the University of Verona, we decided to organise a series of short seminars on topics related to the current activity of the Alumni, be it education, corporate operations, pure or applied research.
The seminar series is called **"Veronesi Tutti Math"**.

The seminars are **short**, **topical**, **interesting**, **informal** and **targeted** to all the alumni. They will take place after dinner (9pm in central european time) and will be organised in 30/40 minutes of talk and 20/30 minutes of discussion. We will close the seminar at 10pm.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}/assets/img/almath-dipartimento.png">
    </div>
</div>

<br><br>
<div class="projects grid">

  {% assign sorted_projects = site.seminars | sort: "importance" %}
  {% for project in sorted_projects %}
  <div class="grid-item">
    {% if project.redirect %}
    <a href="{{ project.redirect }}" target="_blank">
    {% else %}
    <a href="{{ project.url | relative_url }}">
    {% endif %}
      <div class="card hoverable">
        {% if project.img %}
        <img src="{{ project.img | relative_url }}" alt="project thumbnail">
        {% endif %}
        <div class="card-body">
          <h2 class="card-title text-lowercase">{{ project.title }}</h2>
          <p class="card-text">{{ project.description }}</p>
          <div class="row ml-1 mr-1 p-0">
            {% if project.github %}
            <div class="github-icon">
              <div class="icon" data-toggle="tooltip" title="Code Repository">
                <a href="{{ project.github }}" target="_blank"><i class="fab fa-github gh-icon"></i></a>
              </div>
              {% if project.github_stars %}
              <span class="stars" data-toggle="tooltip" title="GitHub Stars">
                <i class="fas fa-star"></i>
                <span id="{{ project.github_stars }}-stars"></span>
              </span>
              {% endif %}
            </div>
            {% endif %}
          </div>
        </div>
      </div>
    </a>
  </div>
{% endfor %}

</div>
