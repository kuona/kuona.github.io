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

{% image 700xAUTO screen-shots/kuona-build-summary-page.png alt="Server summary page" %}

First off the activity chart - shows the number of builds per month for the last year.
{% image 700xAUTO screen-shots/kuona-build-activity.png alt="Build activity" %}

Short builds are important to make sure the feedback is delivered quickly...

{% image 700xAUTO screen-shots/kuona-build-by-duration.png alt="Build by duration" %}

Build outcomes. Success and failure are useful. A high proportion of failures or successes might indicate a problem.

{% image 700xAUTO screen-shots/kuona-build-by-result.png alt="Build by result" %}

What caused the builds

{% image 700xAUTO screen-shots/kuona-build-by-trigger.png alt="Builds by trigger" %}

And finally where the data came from

{% image 700xAUTO screen-shots/kuona-ci-server-summary.png alt="Server summary widget" %}
