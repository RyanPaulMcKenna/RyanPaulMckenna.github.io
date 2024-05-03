---
layout: page
title: Projects
subtitle: A list of personal projects.
---

{% for repository in site.repositories %}
    {%- assign repository_url =  site.github.repository_url | replace: 'RyanPaulMcKenna.github.io', repository.url -%}
    [{{ repository.name }}]({{repository_url}}) {{ repository.summary }}
    <img src="{{repository.image}}" style="display:block;width:250px;border-radius:5%;"  /> 
{% endfor %}


