---
layout: post
title:  "How to install PNDA on AWS"
date:   2017-09-21 22:09:00 -0400
categories: blog
---
### What is PNDA?
PNDA is a Linux Foundation Collaborative Project. It brings multiple open source technologies together, in a manner of providing a scalable and open big data analytics Platform. For more details, have a look at the project's website [here](http://www.pnda.io).

### Installation procedure
## Overview
This blog post is focused on AWS deployment. However, this overview explains the different ways PNDA can be installed. Keep in mind that different types of hosts have slightly different installation procedures.

PNDA can be installed on 4 types of hosts:
* Amazon AWS using CloudFormation
* OpenStack using Heat
* Bare metal using OpenStack tools (Ironic and Heat)
* Virtual Machine using red-pnda

The Virtual Machine installation is not suited for production use, and only provides a minimal set of components so developers can test their applications targeted at a full PNDA stack.

For the other deployments, PNDA provides two pre-configured flavors: Pico and Stardard.
* Pico: Intended for development and learning purposes. It's a fully fledged PNDA software but does not run core services in high-availability mode and provides limited storage.
* Standard: Intended for meaningful PoC and investigations at scale. It runs the core services in high-availability mode and provides reasonable storage and compute resource.

For production deployments and specific needs, flavors can be customised.

Finally, the installation procedure has 6 main steps:
1. Choose and prepare a host
2. Create mirror components
3. Build components
4. Stage components through the mirror
5. Configure the cluster creation process
6. Create the PNDA cluster

You might wonder... Why so many steps? Can't I just run a binary? Well, as many businesses and real world deployments, having internet on a production system is not always an option. Also, online resources are not always dependable. The custom mirror can provides a secure and private way of deploying the application, if used properly.

I see it like the [Gentoo philosophy](https://www.gentoo.org/get-started/philosophy/). It's about using a tool as we see fit, providing maximum flexibility for our needs. The mirror and configuration system provides choices to the administrator that installs PNDA.

PNDA is also still in it's infancy, and will hopefully provide other ways to install the software.

## Installation steps
I will do my best to keep the procedures copy/paste friendly. Keep in mind that this is for PNDA version 3.5, and further releases may provide different steps.

# 1. Choose and prepare a host
TODO
# 2. Create mirror components
TODO
# 3. Build components
TODO
# 4. Stage components through the mirror
TODO
# 5. Configure the cluster creation process
TODO
# 6. Create the PNDA cluster
