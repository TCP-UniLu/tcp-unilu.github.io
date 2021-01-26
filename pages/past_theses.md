---
layout: "page"
title: Past PhD Theses
permalink: "/past_theses/"
---

<h1>Something </h1>

<ul>
{% for thesis in site.data.phd_theses %}
    <h2> {{ thesis.author }} </h2>
    {{ thesis.title }} 
    {{ thesis.University }} 
    {{ thesis.year }}
    {{ thesis.abstract }}
{% endfor %}
</ul>

And some random text here 
