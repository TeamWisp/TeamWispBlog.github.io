---
layout: post
title:  "Our first milestone"
date:   2019-02-22
author: Team Wisp
categories: Devlogs
cover:  "/assets/posts/2019-02-22-first-milestone/sub_temple_4k.jpg"
---

At our university, we work in so-called "blocks". You may know them as trimesters. After working on this project for one trimester, we presented the results of our work to other students and the teaching staff.

The rendering framework is coming together nicely. We currently support three rendering pipelines:
- Deferred (100% rasterization techniques)
- Hybrid (combining deferred with ray-traced shadows and reflections)
- Full RT (100% ray-traced images)

As far as features go, the following features are now supported by the framework:
- Ray-traced shadows.
- Ray-traced reflections.
- Physically-based materials.
- Point, spot, directional lights.