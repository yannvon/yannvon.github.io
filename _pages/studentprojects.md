---
layout: page
permalink: /studentprojects/
title: student projects
description: 
semesters: [on-going,2025,2024,2023,2022] # "pre-print" could be added here.
nav: true
nav_order: 3

---

<p> I always enjoy coming up with new student projects and seeing them through. Check out <a target="_blank" href="https://disco.ethz.ch/theses">our group's website</a> for available student projects or contact me with your own ideas. 


<p> Project reports can be found on my <a target="_blank" href="https://disco.ethz.ch/members/yvonlanthen">university webpage</a>. 

 <!-- _pages/studentproject.md -->
<div class="studentprojects">

{%- for y in page.semesters %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f current -q @*[semester={{y}}]* %}
{% endfor %}

</div>