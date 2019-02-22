---
layout: post
title:  "Our first milestone"
date:   2019-02-22
author: Team Wisp
categories: Devlogs
cover:  "/assets/posts/2019-02-22-first-milestone/sub_temple_4k.jpg"
---

At our university, we work in so-called "blocks". You may know them as trimesters. After working on this project for one trimester, we presented the results of our work to other students and the teaching staff. Our next major project milestone is scheduled for roughly 6 weeks for now.

### Wisp rendering framework updates
The rendering framework is coming together nicely. We currently support three rendering pipelines:
- Deferred (100% rasterization techniques)
- Hybrid (combining deferred with ray-traced shadows and reflections)
- Full RT (100% ray-traced images)

As far as features go, the following features are now supported by the framework:
- Ray-traced shadows.
- Ray-traced reflections.
- Physically-based materials.
- Point, spot, directional lights.

The main feature we were showing-off at the presentation were shadows and reflections <b>IN</b> reflections. This effect can be seen in the banner image at the top of this post.

### Maya viewport plug-in updates
The Maya plug-in has come a long way this trimester. We started without any prior experience with the Maya API, so getting things to work was a bit tricky. Luckily, [Fredrik Linde](https://github.com/Draketuroth) open-sourced a cool [project](https://github.com/Draketuroth/Maya-Custom-Viewport-Renderer) of his. We used this to see how data could be extracted from Maya using a plug-in.

Currently, the plug-in only works with our deferred renderer. We can load models on startup, but there is no dynamic modeling yet. We plan to have this fixed and working properly within a couple weeks.