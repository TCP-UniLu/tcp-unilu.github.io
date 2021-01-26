---
layout: "page"
title: TCP Members
permalink: "/tcp_members/"
---
Below the list of the present TCP goup members. 

A list of the former members can be found <a href="/former_tcp_members/">here</a>

<h1> Post Doctoral Members </h1>
<ul>
{% for member in site.data.people %}
	{% if member.title == "Post-Doc" %}
        <h2> {{ member.name }} {{ member.surname }} </h2>
        <h4>{{ member.title }} </h4>
        <a href="{{ member.google_scholar }}" target="_blank">Google Scholar</a> 
        {% if member.research_interests %}
            <h4> Research Interests </h4>
                {% if member.research_interests[0] %}
                    <ul>
                    {% for entry in member.research_interests %} 
                        <li> {{ entry.item }} </li>
                    {% endfor %}
                    </ul>
                {% else %}
                    <ul>
                        {{ member.research_interests}}
                    </ul>
                {% endif %}
        {% endif %}
        {% if member.expertise %}
            <h4> Expertise </h4>
                {% if member.expertise[0] %}
                    <ul>
                    {% for entry in member.expertise %} 
                        <li> {{ entry.item }} </li>
                    {% endfor %}
                    </ul>
                {% else %}
                    <ul>
                        {{ member.expertise}}
                    </ul>
                {% endif %}
        {% endif %}
        {% if member.past_experience[0] %}
            <h4> Past Experience </h4>
                <ul>
                    {% for entry in member.past_experience %}
                        <li> {{ entry.position }} {{ entry.period }} {{ entry.institute }} </li>
                    {% endfor %}
                </ul>
        {% endif %}
        
        {% if member.Education %}
            <h4> Education </h4>
                <ul>
                    {% for entry in member.Education %}
                        <li> {{ entry.period }} : {{ entry.title }}, {{ entry.institute }}, {{ entry.field }} </li>
                    {% endfor %}
                </ul>
        {% endif %}
        
        <hr style="color:red;height:2px;background-color:red; opacity:60%">
    {% endif %}

{% endfor %}

<h1> PhD Students Members </h1>

{% for member in site.data.people %}
	{% if member.title == "PhD Student" %}
        <h2> {{ member.name }} {{ member.surname }} </h2>
        <h4>{{ member.title }} </h4>
        <a href="{{ member.google_scholar }}" target="_blank">Google Scholar</a> 
        {% if member.research_interests %}
            <h4> Research Interests </h4>
                {% if member.research_interests[0] %}
                    <ul>
                    {% for entry in member.research_interests %} 
                        <li> {{ entry.item }} </li>
                    {% endfor %}
                    </ul>
                {% else %}
                    <ul>
                        {{ member.research_interests}}
                    </ul>
                {% endif %}
        {% endif %}
        {% if member.expertise %}
            <h4> Expertise </h4>
                {% if member.expertise[0] %}
                    <ul>
                    {% for entry in member.expertise %} 
                        <li> {{ entry.item }} </li>
                    {% endfor %}
                    </ul>
                {% else %}
                    <ul>
                        {{ member.expertise}}
                    </ul>
                {% endif %}
        {% endif %}
        {% if member.past_experience[0] %}
            <h4> Past Experience </h4>
                <ul>
                    {% for entry in member.past_experience %}
                        <li> {{ entry.position }} {{ entry.period }} {{ entry.institute }} </li>
                    {% endfor %}
                </ul>
        {% endif %}
        
        {% if member.Education %}
            <h4> Education </h4>
                <ul>
                    {% for entry in member.Education %}
                        <li> {{ entry.period }} : {{ entry.title }}, {{ entry.institute }}, {{ entry.field }} </li>
                    {% endfor %}
                </ul>
        {% endif %}
        
        <hr style="color:blue; height:2px; background-color:blue; opacity:60%">
    {% endif %}

{% endfor %}


</ul>

