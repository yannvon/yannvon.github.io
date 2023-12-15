---
layout: page
permalink: /studentprojects/
title: student projects
description: 
semesters: [on-going,2023,2022,2021] # "pre-print" could be added here.
nav: true
nav_order: 3

---

<p> Check out <a target="_blank" href="https://disco.ethz.ch/theses">our group's website</a> for available student projects. 


<p> Project reports can be found <a target="_blank" href="https://disco.ethz.ch/members/yvonlanthen">here</a>. 

 <!-- _pages/studentproject.md -->
<div class="studentprojects">

{%- for y in page.semesters %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f current -q @*[semester={{y}}]* %}
{% endfor %}

</div>