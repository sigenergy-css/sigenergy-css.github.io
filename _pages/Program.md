---
layout: page
title: Program
permalink: /program
nav: true
---

The workshop features invited talks and a panel discussion. 
Each talk will be 40 minutes long, followed by 5 minute Q&A. 
The panel discussion will last for an hour. 


{% for item in site.data.authors %}



<!-- 
**{{ item.name }}**

**Title:** {{ item.title}} 

**Abstract:** {{ item.abstract}} 

**Bio:**    {{ item.bio }} 
-->

<div class="author-container">
{% if item.img %}
<img class="author-img" src="/assets/img/{{item.img}}">
{% endif %}
<p class="author-name"> <strong> {{ item.name }}  </strong>   </p>
<p>  <strong> Title: </strong>  {{ item.title}}   </p>
<p> <strong> Abstract: </strong>  {{ item.abstract}}   </p>
<p> <strong> Bio: </strong>    {{ item.bio }}   </p>
</div>

{% endfor %}

<br> More details about the speakers, talks, and panel discussion will be available soon.
