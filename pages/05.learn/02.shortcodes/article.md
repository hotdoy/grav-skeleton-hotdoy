---
title: Shotcodes
media_order: sc.svg
subtitle: 'Discover the shortcodes included with Hotdoy.'
image_alt: 'Shortcode tag'
image_width: site
date: '21:33 26-11-2019'
taxonomy:
    author:
        - hotdoy
process:
    markdown: true
    twig: false
shortcode-core:
    active: false
---

This article cover shortcodes included with the Hotdoy theme.
You will need the [Shortcode Core Plugin](https://github.com/getgrav/grav-plugin-shortcode-core) installed properly and setup.
If you still need to install it, you can do it from the Grav Admin Panel under Plugins. Then by clicking Add+ (top right) and searching for it by name.  
Make sure you set the **Custom Shortcodes** path to: 

```/user/themes/hotdoy/shortcodes```

<hr>

## Breakpoint
You can show content on specific devices

```[portrait][/portrait]```

```[landscape][/landscape]```

<hr>

## Buttons
Add buttons.

```[btn href="/my/site-url.com/"]label[/btn]```

```[link href="/my/site-url.com/"]label[/link]```

You can also add the ```mi=""``` attribute to add any [Material Icons](https://material.io/resources/icons/?style=baseline) you might want.

<hr>

## Embed
Add embeded videos from YouTube or Vimeo.

```[youtube="https://www.youtube.com/watch?v=dQw4w9WgXcQ"]```

```[vimeo="https://vimeo.com/148751763"]```

<hr>

## Note
Prevent the rendering of content on the front-end by wrapping anything in the [note] shortcode.

```[note]```
This content will not appear on the front end.
```[/note]```

<hr>

## Material Icons
Add [Material Icons](https://material.io/resources/icons/?style=baseline) 

```[mi="icon-code"]```

<hr>

## Width
In some context, the width of the page is not controlled by the theme and requires you to take those decisions.
You can then wrap your content any available width shortcodes.

```[site][/site]```

```[tight][/tight]```

<hr>

## Swiper
Add a modern touch slider using the great [Swiper](https://swiperjs.com/) library.  
The implementation currently only supports images.

```[swiper]```

```![](scjpg.jpg)```

```![](scjpg.jpg)```

```![](scjpg.jpg)```

```[/swiper]```

<hr>

## Text Size

You can change the size of the text with one of the 4 context (other than the current one) provided by the theme, by wrapping your content with these shorcodes.

```[small][/small]``` (14px)

```[xsmall][/xsmall]``` (12px)

```[big][/big]``` (24px)

```[huge][/huge]``` (48px)

<hr>

## Reveal

Wrap any content to add "reveal" transition..
The default transition will be used if you dont specify any.

```[reveal="my-transition"][/reveal]```

[delays](https://github.com/hotdoy/grav-theme-hotdoy/blob/master/css/delays.css) and [durations](https://github.com/hotdoy/grav-theme-hotdoy/blob/master/css/durations.css) are referenced on github. All times are in milisecond.

<hr>

For more information on the shortcodes providded by the plugin, you can read the offical documentation from the [README](https://github.com/getgrav/grav-plugin-shortcode-core/blob/develop/README.md).
If you find a shortcode from the plugin is unsupported by the Hotdoy theme and would like to sponsor it's addition, you can [open an issue on github on the theme repo](https://github.com/hotdoy/grav-theme-hotdoy)