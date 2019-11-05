---
title: Modular
media_order: 'abstract-page-is-under-construction.png,taxi-page-under-construction.png'
date: '13:53 24-10-2019'
---

![](taxi-page-under-construction.png)

Everything talked aout here will take into account that you are familiar with [Twig](https://twig.symfony.com/doc/2.x/), [CSS variables](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties), the general [structure of a Grav theme](https://learn.getgrav.org/16/themes) and [theme inheritance](https://getgrav.org/blog/theme-development-with-inheritance).

## Available templates

* Splash
* Hero
* Content
* Video
* Drawers

Every modular is a extended partial. In order to extend an existing Modular, simply duplicate the modular template in the child theme. 
All available blocks and variables (sets) are already commented for you. 
Here is what you get in ```/modular/hero.html.twig``` as an example.

[site]
```
{% extends '/partials/hero.html.twig' %}

{# 
{% set video = video|default(page.header.video ? page.media[page.header.video]) %}
{% set image = image|default(page.header.image ? page.media[page.header.image]) %}
{% set image_width = image_width|default(page.header.image_width) %}
{% set image_alt = image_alt|default(page.header.image_alt) %}
{% set reverse = reverse|default(page.header.reverse) %}
{% set rythm = rythm|default(page.header.rythm) %}
{% set reveal_content = reveal_content|default('fadeinfrombottom delay-250 duration-1000') %}
{% set reveal_media = reveal_media|default('fadeinfrombottom duration-1000 delay-200') %}
{% block content %}{% endblock %}
{% block media %}{% endblock %}
#}

```
[/site]

You can then change the values mapped in each variable. Or completely overwrite blocks of the template.
A neat trick could be to extend a block with the [```parent()``` function](https://twig.symfony.com/doc/2.x/functions/parent.html). It this case for exemple, you could add a link after the content with something like...

[tight]
```
{% block content %}
	{{ parent() }}
	<a href="mylink.com">My link</a>
{% endblock %}

```
[/tight]
**Do not modify the equivalent ```/partials/hero.html.twig``` as it will break if any changes are made in future updates.**

