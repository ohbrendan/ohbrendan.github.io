---
layout: page
title: Labs
---

Oh Brendan is a big place. Check out projects which is current being carried out or
[visit Achieves]({{site.base_url}}/labs/achieves.html)

## Startups

{% assign current_tag = 'startuplabs' %}

{% for item in site.categories['labs'] %}
{% for tag in item.tags %}
{% if tag == current_tag %}

### [{{ item.title }}]({{ item.url }})
{{ item.content | split: '<!---more-->' | first }}

{% endif %}
{% endfor %}
{% endfor %}

## Organizations

{% assign current_tag = 'organizationlabs' %}

{% for item in site.categories['labs'] %}
{% for tag in item.tags %}
{% if tag == current_tag %}

### [{{ item.title }}]({{ item.url }})
{{ item.content | split: '<!---more-->' | first }}

{% endif %}
{% endfor %}
{% endfor %}

## Events

{% assign current_tag = 'eventlabs' %}

{% for item in site.categories['labs'] %}
{% for tag in item.tags %}
{% if tag == current_tag %}

### [{{ item.title }}]({{ item.url }})
{{ item.content | split: '<!---more-->' | first }}

{% endif %}
{% endfor %}
{% endfor %}

## Programming

{% assign current_tag = 'programminglabs' %}

{% for item in site.categories['labs'] %}
{% for tag in item.tags %}
{% if tag == current_tag %}

### [{{ item.title }}]({{ item.url }})
{{ item.content | split: '<!---more-->' | first }}

{% endif %}
{% endfor %}
{% endfor %}