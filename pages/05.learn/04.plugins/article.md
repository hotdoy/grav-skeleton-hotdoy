---
title: Plugins
media_order: plugins.svg
subtitle: 'A list of plugins you should install to take advantage of the hotdoy theme'
image_alt: 'some Matrix shit '
image_caption: 'randomly stumbled upon on the web'
image_width: site
date: '07:42 07-02-2020'
taxonomy:
    author:
        - hotdoy
---

The Hotdoy theme takes advantage of a set of plugins and builds upon them.
When installing this theme, one of the first thing you should do is head to the Plugins section and start installing what you need.

## Required plugins

### Admin Panel
Adds an advanced administration panel to manage your site

### Form
Enables forms handling

### Error
Displays error pages.

### Email
Enables the emailing system for Grav

### Login
Enables user authentication and login screen.

### Problems
Detects and reports problems found in the site.

### Admin Addon User Manager
A simple admin panel extension which adds the option to manage users and groups

### Pagination
Paginate collections.
**"Set Use built in CSS" to Disabled**

### Shortcode Core
This plugin provides the core functionality for shortcode plugins.

## Recommended Plugins

### AdvancedPageCache
Statically cache pages but prevent interactivity.
I personally use Cloudflare Page Rules (Cache Everything) but this can be a quick and easy way to boost the speed of certain pages.

### Auto Date
Having a date set in a page never hurts.

### Custom CSS
Quick and dirty fix on the go. Can also be pretty usefull combined with reveal animations included with the theme.

### Data Manager
Adds an admin panel to visualize all kind of saved data.

###  DevTools
Plugin and Theme scaffolding utilities for Grav development. Used for extending theme using inheritance.

###  Markdown Notices
Adds the ability to render notices blocks in Markdown.
Make sure to **turn off "Use built-in CSS"** since the Hotdoy theme has it's own rules to display notices.
Level Classes included in theme:
* yellow
* red
* blue
* green
* dev

### PreCache
Uses Grav's powerful ```onShutdown``` event to run through all pages and call the ```content()``` method of each page.
In other words, cache the whole site when 1 page is hit.

### Quick Tray Links
Easily add cusotmizable admin quick tray links.
Adding Material Design Icons, Grav docs, or other services you use often is a nice touch.

### Sitemap
Add an XML sitemap to your site.