---
layout: post
title:  "Clarisse AOV(LPEs) 设置"
date:   2018-06-03 20:31:54
categories: Clarisse
tags: clarisse aov LPE
---

* content
{:toc}

Clarisse 支持 LPEs（AOV）之后，整理分享一些




## 比较常用的

```
key light = C.*<L.'key_light'>

diffuse = CD.*<L.'key_light'>
diffuse direct = CD<L.'key_light'>
diffuse indirect = CD.<L.'key_light'>
diffuse (without volume and sss) = C<RD[^'sss']>.*<L.'key_light'>

reflection = CS.*<L.'key_light'>
reflection direct = CS<L.'key_light'>
reflection indirect = CS.<L.'key_light'>

glossy = CG.*<L.'key_light'>
specular = C([ST].*)|(G.*)<L.'key_light'>
sss = C<RD['sss']>.*<L.'key_light'>
volume = CV<L.'key_light'>

environment = C.*<' environment_light'>
emission = C.*O

```

