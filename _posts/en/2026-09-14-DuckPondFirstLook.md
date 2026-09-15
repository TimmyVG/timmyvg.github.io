---
title: Primer vistazo a Duck Pond
date: 2026-09-13 10:00:00 +0200
categories: [Blogs]
tags: [blog,godot]     # TAG names should always be lowercase
description: Segundo intento de juego indie
lang: en
page_id: Duck1
image: /assets/img/HopShop.png
projects:
  - duck-pond
---


## What Duck Pond means to me

This game is one of the foundations for forming tinyrawr, the idea being to start building a team that works in harmony.

One of the first difficulties we ran into was getting everyone to share the same idea of a game that doesn't exist yet — even making sketches in Paint and explaining it over long Discord calls, we couldn't bring a consistent version of this idea into the tangible world.

{% include embed/youtube.html id='_V7SS0QO9Fc' %}

So I first tried programming to get a playable version, to have something concrete that would be the same for everyone, and then we complemented it by creating a Miro board.
![Explanatory image of how we use the Miro board](/assets/img/MiroImg.png)

I'm using the [YARD plugin](https://godotengine.org/asset-library/asset/4837) to try to make things more comfortable for Arya (the designer). So far it's been more theoretical than practical, but we're starting to work with it now. I'm not sure whether this is better than a JSON setup with some Python tool for adjusting values — I don't have it fully figured out yet, I'll keep adapting based on results and the designer's feedback.

![Explanatory image of how we use the Miro board](/assets/img/BBDD.png)

A pooling system has been developed for spawning ducks to optimize the game, though there are still many more improvements needed for the incrementals, since things are about to get pretty crazy.
