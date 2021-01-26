---
layout: "page"
title: Collaborators
permalink: "/collaborations/"
---

<h1>
	Ongoing Collaborations
</h1>


Whatever 

<ul>
{% for member in site.data.collaborators %}
    <li> {{ member.name }} {{ member.surname }} {{ member.institute }} </li>
{% endfor %}
</ul>
