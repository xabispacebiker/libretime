---
layout: default
title: Built-in Microsite
git: microsite.md
---

## Overview

![](img/radio-page.png)

LibreTime includes a mini-site, which can be accessed at _serverIP_ (for local installations), or
_libretime.yourdomain.com_ or _cloudvmIP_ (for installations to a server on a domain). The site includes your
logo and station description (set under Settings > General), the login button to the LibreTime interface, the schedule for the next seven days,
podcast tabs, and a live feed of your station with the currently playing artist and track displayed.

## Modifying the LibreTime Radio Page

The background of the mini-site that appears when you visit the server's domain in your web browser can be changed by modifying the page's CSS file, located at */usr/share/airtime/php/airtime_mvc/public/css/radio-page/radio-page.css*.

```
html {
    background: url("img/background-testing-3.jpg") no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    overflow-y: auto;
}
```

Place the new background image in the */usr/share/airtime/public/css/radio-page/img/* folder and change the `background:` entry's URL to point to the new image. The new image should be at least 1280 x 720 in pixel size to avoid being blurry.
