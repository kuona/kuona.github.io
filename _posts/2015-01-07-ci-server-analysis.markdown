---
layout: post
title:  "Kuona CI analysis"
date:   2015-01-07
categories: status
---

The first goal for Kuona is to collect data about CI server activity
and chart it in a way that can provide insight into the effectiveness
of the system.

Here are some example screen shots from my Jenkins CI server that I use for personal projects.

![Server summary page](/images/screen-shots/kuona-build-summary-page-700.png)

First off the activity chart - shows the number of builds per month for the last year.

![Build activity](/images/screen-shots/kuona-build-activity-700.png)

Short builds are important to make sure the feedback is delivered quickly...

![Build by duration](/images/screen-shots/kuona-build-by-duration-700.png)

Build outcomes. Success and failure are useful. A high proportion of failures or successes might indicate a problem.

![Build by result](/images/screen-shots/kuona-build-by-result-700.png)

What caused the builds

![Builds by trigger](/images/screen-shots/kuona-build-by-trigger-700.png)

And finally where the data came from

![Server summary widget](/images/screen-shots/kuona-ci-server-summary-700.png)
