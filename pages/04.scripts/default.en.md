---
title: Scripts
---

## Reveal
Add "reveal" animation to any element by adding ```data-reveal``` to it.
A default fadein will then be added when the element enters the screen.
You can learn more about this on [Github](https://github.com/hotdoy/reveal.js/blob/master/README.md) 

## links
Small link manager. Mostly to add or remove attributes.
Add ```target="_blank"``` to link starting with ```http``` by default.

## slow3g
User facing utilities for slow networks.
Comprised of 3 files.

**slow3g.js**  
Warn users 2 seconds after a link is clicked if nothing happens by adding a full page overlay blocking further interaction and preventing more request.

**slow3g.html.twig**  
Slow network message template.

**slow3g.css**  
Styles for the message template. Also add some loading effects background on images (ommiting transparency enabled fomats) and videos. You can prevent this by adding the ```no3g``` class on said elements.

## site-header
Default site header / menu.
* site-header.js
* site-header.html.twig
* site-header.css

## site-loader
Default site-loader / transitions.
* site-loader.js
* site-loader.html.twig
* site-loader.css

## video
Pause or play videos depending on their visibility.

## notify
User facing notification system.

## form
Submits forms trough ajax. Then notify the user using notify.js