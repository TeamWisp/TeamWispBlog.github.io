---
layout: post
title:  "February progress update"
date:   2019-03-01
author: Team Wisp
categories: Updates
cover:  "/assets/posts/2019-03-01-progress-update/bistro_4k.jpg"
---

About three weeks ago, a new trimester started for all of us. Because we had show results last block, the project had accumulated some technical debt. We decided to spend the first two to three weeks of the block on refactoring.

### Summary
#### Wisp rendering framework
- Lots of bug fixes.
- Ray-traced soft shadows.

#### Wisp Maya plug-in
- Codebase refactoring.
- Moved to using Maya modules to install the plug-in.
- Viewport resizing.

### Framework
The team working mainly on the Wisp rendering framework managed to solve a lot of issues and bugs. It's not a lot more stable and easier to use. Additionally, readback buffers have been fixed as well. They now support textures that are not a perfect multiple of 256 wide. Padding is applied automatically when needed.

Meine has been working a lot on improving the quality of the ray-traced shadows. The rendering framework now supports ray-traced soft shadows! At the end of the week, Darius managed to get a first version of depth of field to work! This feature will be supported by the Maya plug-in soon.

### Maya
While the Wisp team was working on fixing issues and bug in the framework, the Maya team decided to start reworking the plug-in. The plug-in is now structured properly (added custom user operations, parser classes, split-up huge files, ect.).

Additionally, we switched to Maya modules! This means you no longer have to place Wisp resource files inside the Maya installation folder.