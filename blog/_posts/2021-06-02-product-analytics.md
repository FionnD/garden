---
layout: post
title: Product Analytics for Product Managment
truncated_preview: true
excerpt_separator: <!--more-->
---

A splattering of thoughts on product analytics and their connection to the role of product managment.

I remember reading somewhere that the three stages of product management are:

1.  Planning a product (User interviews etc)
2.  Building a product
3.  Tracking a product

This plan, do, track methodology can be employed for each release in a product cycle. For example, did our conversion rate increase after the last release? If not, maybe we misunderstood the user during the planning process etc. etc.

Generally, things you track are called KPI, which is one of those words that have taken on it's own life after being shouted in the boardroom one too many times. If you have a lot of KPIs, you might consider using a single north start KPI.

  KPIs can be normally divided into (regardless of B2B or B2C)

1.  Acquisition
2.  Retention
3.  Engagement (measured in daily active users & monthly active users)
4.  Revenue

 It is generally assumed that in the long run, `Revenue is a function of (Acquisition -> Retention -> Engagement)`. 73.6% of All Statistics Are Made up, so numbers should always be taken with a healthy grain of salt. Generally, if these numbers are rising, things are A-OK, if they are dropping, it's time to do a retro on the topic.

 ## Additional thoughts on KPI for commercial open source projects.

**Acquisition** should capture all the reasonable ways a user could install your product. Some common ones are:

`a` = pip install tensorflow
`b` = Git clone google/tensorflow
`c` = Docker pull tensorflow

Where `acquisition = a + b + c`

**Retention** for a COSS product is tough to measure without tracking individual user behavior within your product. Some frameworks employ telemetry tracking, Rasa is an example. Engagement, in the past, I have used the following formula for this.

`a` = Github issues opened per month (by people not part of the commercial team)
`b` = Github pull requests opened per month

    engagement = a + b
