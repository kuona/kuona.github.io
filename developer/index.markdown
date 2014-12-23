---
layout: default
title: Developer Guide
---

# Developer Guide

This guide should help get you up and running developing Kuona
additions or bug-fixes.

This is *very* early documentation and change is likely - this also
means that we can take the project into new and interesting areas so
please make your suggestions and send in those pull requests!

## Getting Started

Kuona is pretty much self contained. You will need a valid Java 1.8
JDK and Git. Either fork or clone git@github.com:kuona/kuona.git. The
root directory contains a thin wrapper for the build called
_run_. It's a thin wrapper around the bundled [ant](http://ant.apache.org)
build tool.

	run -p

lists the available targets.

*run* with no parameters runs the default _test_ target.

Dependencies are managed in version control. Everything from the build
system to the required libraries. This makes is more complex to update
and a little longer to check out but much easier to get started and
build regularly.

*Note* At the time of writing there are a couple of problems with the
 command line test target. IntelliJ and CI (Jenkins) handles things
 fine so I suggest double checking with the IDE. Something to get
 sorted soon.

## Finding your way around

[KuonaSpecTests.java](https://github.com/kuona/kuona/blob/master/src/test/java/kuona/config/KuonaSpecTests.java)
is probably a good place to start reading code. Much of Kuona's
behaviour is driven by the configuration file.

Kuona is a batch oriented system. It retrieves and locally stores data
in the original CI or VCS system for later analysis. By storing the
data in an original text format it makes it easier to invent new data
processors and account for infrastructure changes. Data retrieved from
systems is stored locally on the file system.

[ProcessorBuilderTests.java](https://github.com/kuona/kuona/blob/master/src/test/java/kuona/processor/ProcessorBuilderTests.java)
is a good place to start when adding a new processor (something that
can read and analyse a systems data).
