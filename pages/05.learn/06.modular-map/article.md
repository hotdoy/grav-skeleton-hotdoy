---
title: 'Modular: Map'
media_order: maps.svg
subtitle: 'Adding Google Maps to your page using the Map modular.'
image_alt: 'map pin'
image_width: site
date: '08:19 09-02-2020'
---

The "Map" modular is ... well, a modular. This means that in order to add it to a page, the said page must support modular pages.
If you don't know about modular pages, here is the [official documentation](https://learn.getgrav.org/16/content/modular).
I also coverred adding your first modular [here](https://hotdoy.ca/learn/modular/).

## Get started with Google Maps Platform

You will need to: 
* Create a billing account
* Create a project
* Enable one or more APIs or SDKs
* Get, add, and restrict an API key

While I won't go in detail as to what setup you need on the Google side, your fist stop should be [this tutorial from Google](https://developers.google.com/maps/gmp-get-started).

## Adding the map

Once you have a valid API key. You should head to the Hotdoy theme configuration:

* Go to the Themes page of the Grav Admin panel and select Hotdoy.
* Scroll down to the Google Maps section.
* There you can copy your key in the "Google maps API Key" field.
* Hit the "Save" button.

Now that Google Maps is setup, you are ready to add a map modular!

Each coordinates must have:

* A title
* Latitude
* Longitude
* An optional URL to send the user to when the marker is clicked
* An optional custom Icon.

A custom icon can be set for the entire site withing the theme configuration. You can otherwise set a custom icon for each marker by uploading an image directly into the Page Media field in the modular and selecting it with the icon field in each Marker. 
