---
title: 'Recent Posts'
align: left
width: site
date: '07:55 11-02-2020'
margin_top: half
padding_top: none
padding_bottom: none
margin_bottom: none
role: default
limit_reveal: '0'
process:
    markdown: true
    twig: true
twig_first: true
margin: top
padding: none
---

{% for post in page.find('/learn').children.order('date', 'desc').slice(0, 3) %}
	{% include '/partials/article-card.html.twig' with {'page':post} %}
{% endfor %}